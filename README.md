# Booting as root from the bootloader - Linux Kernel

I was once locked out of my machine because I didn't install the config file for my lone window manager (*i was being silly*), so I decided to fix things up :)

While in the process, I thought about sharing how to boot as root and have root permissions.
## Step 1
Turn on your machine, and after being greeted by GRUB bootloader, press E to modify how your machine will boot ( with command )
![1](https://raw.githubusercontent.com/0x7ax/linux-boot-as-root/main/1.png)
## Step 2
Locate the kernel loader, it should be under the name *linux*
![2](https://raw.githubusercontent.com/0x7ax/linux-boot-as-root/main/2.png)
## Step 3
Add *init=/bin/bash* to the end of the kernel loader line
![3](https://raw.githubusercontent.com/0x7ax/linux-boot-as-root/main/3.png)
If the line doesn't contain *rw*, make sure to add it.
After that, press F10 or whatever key it's being binded to to proceed booting
## Demonestration
![4](https://raw.githubusercontent.com/0x7ax/linux-boot-as-root/main/4.png)
## Kernel Panic
It's totally normal for a kernel panic to occur, your progress should be saved.
![5](https://github.com/0x7ax/linux-boot-as-root/blob/main/5.png)
