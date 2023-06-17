## Basic Command On Ubuntu 
1. sudo. 
sudo (SuperUser DO) Linux command allows you to run programs or other commands with administrative privileges, just like “Run as administrator” in Windows.
This is useful when, for example, you need to modify files in a directory that your user wouldn’t normally have access to.
2. List all the packages installed on your system.
If you don’t know the package name, use below ubuntu basic command to list all the packages installed on your system
```
$ dpkg --list
```
3. Apt-Get
apt-get is the one of the most important Ubuntu commands every beginner must know. 
It is used to install, update, upgrade and remove any package.
apt-get basically works on a database of available packages. Here is the list of different apt-get commands:
#### apt-get update
```
$ sudo apt-get update
```
apt-get update with super user privileges is the first command you need to run in any Linux system after a fresh install. 
This command updates the database and let your system know if there are newer packages available or not.

#### apt-get upgrade 
After updating the package database, next step is to to upgrade the installed packages.
For upgrading all the packages with available updates you can use this command.
And if you like to upgrade a particular package, you should tweak the above command a little:
```
$ sudo apt-get upgrade <package-name>
```
Replace the <package-name> with your desired package.

#### apt-get install 
If you know the name of the package, then you can easily install a program using this command:
```
$ sudo apt-get install <package-name> 
```
Replace the <package-name> with your desired package.
If you are not sure about the package name, you can type a few letters and press tab and it will suggest all the packages available with those letters.
Thanks for auto-completion feature.

#### apt-get remove
When it comes to removing the installed program apt-get remove command suits your need. 
You only have to know the exact package name of the software you want to uninstall.

```
$ sudo apt-get remove <package-name>
```
Replace the <package-name> with the one you copied from the dpkg list.
. apt-get remove command only removes the software from your system but not the configuration or data files of the package. 
These files help in keeping the same settings when you want to reinstall the same software.

#### apt-get purge
apt-get purge command is used when you want to remove a software completely from your system with its configuration or data files so that no longer personalized settings will be available during reinstallation.
Run the apt-get purge command as sudo in order to remove the software completely:
```
$ sudo apt-get purge <package-name>
```
Replace the <package-name> with the application that you want to remove or copied from the dpkg list.

#### apt-get autoremove
apt-get autoremove command is used to remove any unnecessary packages. 
Unnecessary means, whenever you install an application, the system will also install the software that this application depends on. 
It is common in Ubuntu that applications share the same libraries. When you remove the application the dependency will stay on your system.
So run apt-get autoremove as sudo after uninstalling a package to remove unwanted software dependencies.
So apt-get autoremove will remove those dependencies that were installed with applications and that are no longer used by anything else on the system.

4. Lists all files and folders in your current working directory on Linux
ls (list) command lists all files and folders in your current working directory. 
You can also specify paths to other directories if you want to view their contents.
```
$ ls
```

5. Change the current working directory on Linux
cd (change director”) Linux command also known as chdir used to change the current working directory. It’s one of the most used basic Ubuntu commands. Using this command is easy, just type cd followed by the the folder name. You can use full paths to folders or simply the name of a folder within the directory you are currently working. Some common uses are:
 – Takes you to the root directory.
```
$ cd /  
```
– Takes you up one directory level.
```
$ cd .. 
```
– Takes you to the previous directory.
```
$ cd –  
```
– Open home folder in current directory.
```
$ cd home
```
– Open Linux Drive named folder in directory.
```
$ cd Linux\ Drive
```
Here you can see I use backslash because the folder name has spaces so for each space you use “backslash+space”. 
Like, if your folder name is “am a programmer” then the cd command will be, “cd am\ a\ programmer”.

6. Ubuntu command displays the full pathname of the current working directory.
```
$ pwd 
```
(print working directory)
7. Linux command allows you to copy a file. 
You should specify both the file you want to be copied and the location you want it copied to
```
$ cp xyz /home/myfiles
```
the file “xyz” to the directory “/home/myfiles”.
8. Move files
You can also rename files by moving them to the directory they are currently in, but under a new name.
```
$ mv xyz /home/myfiles
```
the file “xyz” to the directory “/home/myfiles”.
9.  Command removes the specified file.
– Removes an empty directory.
```
$ rmdir <remove-directory>
```
– Removes a directory along with its content.
```
$ rm -r <remove-recursively>
```
10. Create a new directory
You can specify where you want the directory created – if you do not do so, it will be created in your current working directory.
```
$ mkdir
```
11. Displays all of your previous commands up to the history limit.
```
$ history
```

12. Display filesystem
Command displays information about the disk space usage of all mounted filesystems.
```
$ df
```
13. Directory usage
Command displays the size of a directory and all of its subdirectories.
```
$ du
```
14. Free space available on the system
Displays the amount of free space available on the system.
```
$ free
```
15. Basic information about the system
Provides a wide range of basic information about the system.
```
$ uname -a
```
16. Manual pages are usually very detailed
Manual pages are usually very detailed, and it’s recommended that you read the man pages for any command you are unfamiliar with. 
- Provides information about the manual itself.
```
$ man man 
```
– Displays a brief introduction to Linux commands.
```
$ man intro
```
17. more detailed or precise information
```
$ info
```
18. Change user password 
Ubuntu basic command is used to change user password using Terminal. What you have to do is run the below command, where is the username whose password has to change
```
$ passwd <user>
```
19. Above commands will display the purpose 
```
$ whatis <command>
```
examples are: <command> is cd, man, help ...
20. Ubuntu Terminal Shortcuts
To further ease up your skill, these Ubuntu Terminal keyboard shortcuts would help.
- Open new tab on current terminal : Ctrl + Shift + T
- Close the current tab : Ctrl + Shift + W
- Move cursor to beginning of line : Ctrl + A
- Move cursor to end of line : Ctrl + E
- Clears the entire current line : Ctrl + U
- Clears the command from the cursor right : Ctrl + K
- Delete the word before the cursor : Ctrl + W
- Allows you to search your history for commands matching what you have typed : Ctrl + R
- Kill the current process : Ctrl + C
- Suspend the current process by sending the signal SIGSTOP : Ctrl + Z
- Clears the terminal output : Ctrl + L
- Move forward one word : Alt + F
- Move backward one word : Alt + B
- Copy the highlighted command to the clipboard : Ctrl + Shift + C
- Paste the contents of the clipboard : Ctrl + Shift + V or Shift + Insert
- To scroll through your command history, allowing you to quickly execute the same command multiple times : Up/Down Arrow keys
TAB: 
Used to complete the command you are typing. If more than one command is possible, you can press it multiple times to scroll through the possible completions. If a very wide number of commands are possible, it can output a list of all possible completions.
 
