# BERTLINUX


A lightweight linux distribution built with the "Linux From Scratch" book (version 12.0)

![BERTLINUX](https://github.com/gbertuzzi05/BERTLINUX/assets/106744847/12d48007-3e45-4c46-83ba-041beca3e2bf)





WARINING: i'm just a student who started this project for school reasons i'm not a developer.





I started BERTLINUX with the intention to create an ultra-lightweight operating system that can be used with any computer (with an x86_64 cpu)
I compiled the kernel with general settings and added support for a few drivers
I installed LXDE (Lightweight X11 Desktop Environment) as Desktop Environment and some tools for basic use as a text editors (Bluefish for the desktop, nano and vim for the CLI), a WEB browser (palemoon), process manager (top and htop) and programming tools (gcc, g++ and python3).

the kernel version is 6.4.12 and has been compiled with the default configuration

# WHAT WORKS



the cli and its commands, the desktop environment (LXDE) 

# WHAT PARTIALLY WORKS


internet works only with ethernet port (labelled eth0 according to "ifconfig" command) wpa_supplicant is installed but need Wi-Fi driver
Some peripherals may be detected by the system but may require one or more drivers to be used.
# WHAT IS NOT WORKING


audio, Everything else


# TO LOGIN:

USER:root

PASSWORD:root





# HOW TO USE 



# VM with VirtualBox
-Download and extract the .vdi from releases page (32GB of space are required)


-Create a VM vith virtualbox [type: linux/other-linux(64-bit) , RAM minimum 512 MB and cpu from 1 to max]


-Add the .vdi to the virtual machine


-Boot up and enjoy


# Raw image to hard drive

-connect your hard drive to the pc using a usb adapter

-download the .img file from the releases page (32GB of space are required)

-flash the .img file to hard drive using a flashing tool like balenaEtcher (https://etcher.balena.io/)

-Boot up and enjoy


# LIVE USB

-download and extract the .tar.xz file (with windows you can use 7-zip, with linux you can use "tar -xf" command
-inside you will find the BERTLINUX folder with three subdirectories: boot, changes and modules
-copy the BERTLINUX folder into the root (/) of your usb
-now follow the steps for your OS 


--on WINDOWS run cmd as admin and run this command: "cd /d [letter-of-your-drive]:BERTLINUX/boot" and press enter, then run bootinst.bat (WARNING:this is not equal to "run as administrator from right click menu you need to execute in terminal or will not work



--on LINUX open the terminal as root or as a user in the sudo group and run this command: "cd /path/to/usb/BERTLINUX/boot" and press enter, then run "./bootinst.sh" 
-when the script will end, an "installation finished" message will be prompted and you can close the terminal

# BOOT THE DESKTOP


  To boot desktop withVM METHOR OR RAW IMAGE METHOD issue the command "startx" in the bash, with the LIVE USB method use the liveusb.sh script in the /root folder



-To edit screen resolution use xrandr from cli or lxrandr from gui


