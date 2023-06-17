
 ## [Expand Ubuntu disk] (http://linguist.is/2020/08/12/expand-ubuntu-disk-after-hyper-v-quick-create/)
It is quick and easy to use Hyper-V Quick Create to get an Ubuntu virtual machine running on a Windows 10 computer.
However, if this method is used, you may end up with a tiny Ubuntu virtual disk that will not be useful for any serious work and it is less obvious than the initial setup how to increase the size of this disk.
These steps fix the problem:

Ex: 
```
resize2fs /dev/sda 6000M
```
You have to first resize the partition with the following steps:
1. sudo parted /dev/sda 
to enter the prompt "(parted)" as the superuser
2. resizepart 1 
to resize the partition 1
3. Enter -0 resizes it 
to the end of the disk. - indicates that it should count from the end of the disk, not the start.
This makes -0 the last sector of the disk - which is suitable when you want to make it as big as possible. Step 4:
4. quit 
to exit parted

The file system meta information needs to indicate the size of disk, and resize2fs updates this.
Thus, after expanding, run resize2fs /dev/sda1.

It's highly recommended to do this in either single user mode / recovery mode, or with the file system mounted in read only mode. You can mount it read only by mount -o remount,ro /dev/sda1.

Extending is possible to do with filesystem in RW-mode, but it increases chances of data loss. As this is a VM, and you can easily make a backup, doing it with the volume mounted RW may make sense.

Addendum: run commands as root for desired effect.


It is quick and easy to use Hyper-V Quick Create to get an Ubuntu virtual machine running on a Windows 10 computer. However, if this method is used, you may end up with a tiny Ubuntu virtual disk that will not be useful for any serious work and it is less obvious than the initial setup how to increase the size of this disk.

These steps fix the problem:

Turn off the VM.

Use Hyper-V Manager to select the Settings of the Virtual Machine,
select the Hard Drive option and Edit under Virtual hard disk. 
(If this option is disabled, you need to go back and delete any checkpoints for the VM in the Hyper-V Manager; just select the VM and right click the checkpoint in the checkpoint field below.)
Use the GUI to expand the drive to something reasonable, like 128 GB. Ubuntu now has space to expand into.

Start the VM again. Install Guest Utils:
sudo apt install cloud-guest-utils
If not using English, override locale settings to avoid issues with non-English locales:
LC_ALL=C
Expand the sda1 partition into the free space:
sudo growpart /dev/sda 1
(Note the space between sda and 1!)
Finally run resize2fs:
sudo resize2fs /dev/sda1
(No space between sda and 1 here!)
Now your Ubuntu drive is 128 GB.
