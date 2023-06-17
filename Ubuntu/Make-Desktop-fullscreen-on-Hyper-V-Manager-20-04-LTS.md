

## Make Desktop fullscreen on Hyper-V Manager - Ubuntu 20.04 LTS  
1. Open up the terminal and type
```
sudo nano /etc/default/grub
```
It will ask for administrative password. Simply type that in and enter.
2. Now we should edit the grub as follows.
Change line
```
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash"
```
To
```
GRUB_CMDLINE_LINUX_DEFAULT="quiet splash video=hyperv_fb:1920x1080"
```
Notice that 1920×1080 is your screen resolution. You can change it according to your screen resolution.
Press “Y” to save file.
3. Reboot the system by typing
```
sudo reboot
```
4. Once the system boots up again, open up the terminal and type
```
sudo update-grub
```
5. Reboot the system by typing
```
sudo reboot
```
6. Vim
 Command	Description
Press the ESC key
```
 Type :q!
 Press the ENTER key	Exit vim without saving changes i.e. discards any changes you made.
 Press the ESC key
```
```
Type :wq
Press the ENTER key	Save a file and exit.
Press the ESC key
```
```
Type :x
Press the ENTER key	Save a file and exit.
```
