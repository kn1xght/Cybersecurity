WINDOWS EDITIONS

Many versions of Windows since the 1985, some of the notable mentions being the Windows 95, XP, Vista, 7, 10, 11
Alongside the operating system, exists the Windows Server, current version being 2025. This is the enterprise solution, it's a management software in a nutshell that provides many tools and services to enterprise IT. 
Fun fact if you can't decide between the home and pro version of windows 11, pro version has the ability to use bitlocker device encryption. (basically locks the device completely, preventing anyone else accessing ur system)

INTRODUCTION TO WINDOWS 

Windows 11 GUI (Graphical User Interface)

![Task Manager](images/windows11gui.jpg)

Contains elements such as: 
1. Start Menu
2. Task View
3. Taskbar
4. Toolbars
5. Notification Area

INTRODUCTION TO WINDOWS 

Windows 11 is extremely customizable, it allows you to suit it to your liking (wallpapers, themes, colors etc), one of many perks I like to spend hours of my time on. (oops)

The Start Menu 

Provides access to all apps/programs, files, utility tools etc. You can find it on bottom left corner, in previous versions there was a "Start" word indicating it, newer ones only contain the windows logo within the box. 

The Taskbar

Allows us to enable/disable cool neat features such as news/interests, cortana. I like to have them disabled personally, if left unmanaged, they can start cluttering your screen really quickly.  

The Notification Area

Unlike Start Menu, notification area is to be found on the bottom right of the Windows screen, where the date and time are displayed alongside many other things that can be toggled on/off, some of which include location, touch keyboard, microphone etc.

This short introduction to some of the features Windows contains is only scratching the surface, in reality it is a complex product with many system files, utilities and settings that we will learn about as we dive deeper into the write-ups.

THE FILE SYSTEM

The file system used in modern versions of Windows is the New Technology File System or simply NTFS. 

Before NFTS, we had FAT16/FAT32 (File allocation table) and HPFS(High Performance File System). These can still be seen in use today, typically in USB devices, MicroSD cards etc. It's limitations are addressed by NTFS which were:

Supporting files larger than 4GB
Folder and file compression
Encryption (Encryption File System or EFS)

A very nice feature of the newer NTFS is that it can automatically repair the folders/files on disk using information stored in a log file. FAT doesn't allow for this. 

LESSON: To check what file system OS is using, right click on the drive where OS is installed, typically C drive -> properties -> listed at the top. 

NTFS permissions are as follow:  

![Task Manager](images/ntfs-permissions1.png)

LESSON: To check permissions for files/folders, right click -> properties -> Security tab

Another NTFS feature is Alternate Data Streams (ADS). It allows hidden metadata or additional data to be attached to a file without changing its main contents. For example, telling us whether the file was downloaded from the internet (Zone.Identifier).

THE WINDOWS/SYSTEM32 FOLDERS

The windows folder is known as the folder which contains the Windows Operating system, typically sitting on the C drive for most users, but we're allowed to install it on any driver we wish to. 

System variable for the Windows folder is %windir% (windows directory). One of many folders inside is the "System 32", it holds important files that are critical for the operating system's function. Approach with caution when modifying anything relating to this folder, it can make it inoperational.

USER ACCOUNTS, PROFILES AND PERMISSIONS

On a typical local Windows system they come in 2 flavours: 

Administrator (enabled to make changes to system, add/delete users, modify groups, modify settings etc.)
Standard User (enabled to make changes locally, think folders/files & can't perform system-level changes.)

LESSON: Way to access information on existing users, groups, permissions and much more is to use Local User and Group Management. Right-click on the Start Menu and type in lusrmgr.msc. You should see two folders: Users and Groups, information about existing users/groups etc. will be stored here. 

USER ACCOUNT CONTROL: 

A user doesn't need to run with high (elevated) privileges on the system if the user only wishes to perform tasks such as surfing the internet, working on Word document etc. Elevated privilege increases the risk of system compromise because it makes it easier for malware to infect the system. To prevent this, Microsoft introduced User Account Control (UAC).

How does it work? When a user with an admin account logs into system, the current session doesn't run with elevated permissions. When an operation requiring higher-level privileges needs to executre, the user will be prompted to confirm if they permit the operation to run. 

SETTINGS AND CONTROL PANEL

The primary way to make changes are the Settings and Control Panel menus. 

Let's first take a look at how each looks: 

![Task Manager](images/win-settings.png)

![Task Manager](images/win-control-panel.png)

Control Panel is really the menu where you will access more complex settings and perform more complex actions. 

TASK MANAGER

Provides information about the applications and processes currently running on the system. Also displays information such as how much CPU and RAM are being utilized, which falls under the Performance tab. 
This tool is easily accessible by right-clicking the taskbar. 

CONCLUSION

Even though Windows OS has been my go-to choice over many years now I was still humbled by this short introduction. I came across the UAC "confirm with authenticity" pop-up many times by now, but I never quite knew what was the process behind it. The rest of the information in this room I had came across and was well familiar with, however it doesn't hurt to get a refresher. 