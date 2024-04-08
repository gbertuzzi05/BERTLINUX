# BERTLINUX
A lightweight linux distribution built with the "Linux From Scratch" book (version 12.0)

WARINING: i'm just a student who started this project for school reasons i'm not a developer.
why i have done it?

I created BERTLINUX with the intention of creating an ultra-lightweight operating system that can be used with any computer (with an x86_64 cpu)
I compiled the kernel with general settings and added support for a few drivers
I installed LXDE (Lightweight X11 Desktop Environment) as Desktop Environment and some tools for basic use as a text editors (Bluefish for the desktop, nano and vim for the CLI), a WEB browser (palemoon), process manager (top and htop) and programming tools (gcc, g++ and python3).

the kernel version is 6.4.12 and has been compiled with the default configuration

what works:
the cli and its commands

what partially works:
the screen only works if the kernel is booted up with "nomodeset" option and uses a generic graphic driver with default resolution of 1024x768
internet works only with ethernet port (labelled eth0 according to "ifconfig" command)

what is not working:audio, everithing else and there is no battery management for laptops




system image coming soon




Some peripherals may be detected by the system but may require one or more drivers to be used.

To login use "root" for username and password.

To boot desktop issue the command "startx"
