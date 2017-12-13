# Systems Administration & Configuration
 -
 -    1. Boot process and Troubleshooting
 -    2. Basic System Configuration
 -    3. System Logging
 -    4. Disk Management and File System Creation
 -    5. Managing Linux Users and Groups
 -    6. Linux Networking (setting up networking and config)
 -    7. Process and Job Management
 -    8. Creating, Viewing and Editing Text Files (Vi)
 -    9. Installing and Updating Software Packages
 -    10. Scheduling and Automating Future tasks
 -    11. Network Storage and Management (NFS, SMB)
 -    12. Service Configuration (DHCP, FTP, DNS, SSH, HTTP etc...)    
 -    
 -    Linux Boot Process and Troubleshooting
  
 -### Boot process and Troubleshooting
 +# Elive Linux Basic System Administration
  
 -  1. Three major areas
  
 -     1-BIOS
 -          The first program
 -          Runs from ROM
 -          OS independent
 -	 
 -          Bios does the following two main tasks
 -	  1-POST
 -	   Power on self test
 -	  2-Boot an OS from
 -  	    a storage device
 -	   -Proceed through until it finds an MBR
 -	   a. To go into GRUB config mode, press "e" at the GRUB main screen.
 +### By Mohamed Mohamud and Mohamed Mohamed
  
 -      b. To see the default bootable drive type "echo $root"
 +## Topic Areas
  
 -     2-Bootloader
 -	
 -	-MBR (Master Boot Record)
 -	  first sector of the hard drive
 -	  Bootloader may reside in the MBR
 -	  and or may reside elsewhere
 -	-MBR runs the bootloader
 -	 -Bootloader(Grub, LILO etc..) loads the OS
 -	-May create an initrd image
 -          "Initial ramdisk"
 -
 -
 -     3-Kernel
 -       Bootloader loads the kernel
 -       -/boot/vmlinuz (z at the end means compressed)
 -       -Maybe compressed file 
 -       -linuxrc 
 -         1. linux run command
 -       -initrd ramdisk is dismounted
 -	
 -        -File system is mounted
 -	 Kernel runs init.
 +* Boot Process and Troubleshooting.
 +* Basic System Configuration.
 +* System Logging.
 +* Disk Management and File System Creation.
 +* Linux Networking and Configuration.
 +* User and Group Management
 +* Process and Job Management.
 +* Creating and Editing Text Files.
 +* Installing and Updating Software Packages.
 +* Scheduling and Automating Future Tasks.
 +* Service/Server Configuration (DHCP, FTP, DNS, SSH and HTTP).
 +
 +#### Section 1.1 Boot Process
 +
 +When you first boot an Elive Linux Operating System or any Linux OS it will go through the following processes to boot into the command line or desktop. When you press the power button on a machine that is running Elive, the first program that runs in the BIOS. BIOS stands for Basic Input Output System. We must clarify about the BIOS before we go any further.  To be clear the BIOS is not part of the Linux kernel. The BIOS is separate of the operating system, it is not part of the OS. It can be found on computers running other operating systems such as Windows and others. The BIOS is a software that is built into a computer's ROM (Read Only Memory) at the time of manufacturing the motherboard. The BIOS goes through two main stages to boot a Linux kernel. It first does POST (Power On Self Test). In this first stage the BIOS checks to ensure that peripheral devices are intact and ready to operate the system after boot up. Peripheral devices are things like the keyboard, monitor, mouse, RAM, CPU and so on. Below is a screenshot of a BIOS.
 +
 +*Figure 1.1 BIOS.*
 +
 +
 +The next stage of the BIOS is that it looks for an MBR (Master Boot Record) on all the drives that are connected to the system. The BIOS has a boot menu which lists the boot order of all bootable devices that are available on a given system. Most BIOS by default are configured to check for the MBR on the first disk drive onboard. If there is no disk drive it'll check for a CD/DVD ROM or USB; which basically means it'll go through all the drives that are connected or onboard until it finds a drive with an MBR. Then it hands of the boot process to the drive that has the MBR. Another screenshot of the BIOS's boot menu.
 +
 +
 +*Figure 1.2 BIOS boot menu.*
 +
 +
 +
 +The MBR is the first sector of a disk drive; it holds a table of partitions on the disk drive. The MBR will look all the partitions on the drive to find one that has a boot loader. There are many common boot loaders but Elive linux uses GRUB two. Below is a screenshot of the GRUB two startup menu that is getting ready to boot up an Elive linux. 
  
 +![](GRUB2.png)
 +*Figure 1.3 GRUB Boot Menu.*
  
 -Sources
  
 -https://www.youtube.com/watch?v=mHB0Z-HUauo
 -How linux works text book. 
