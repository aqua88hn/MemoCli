
 ## Expand Ubuntu disk 
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
