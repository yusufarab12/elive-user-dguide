### journal 1	


My three learning-how-to-learn methods are:

	•	Interleaved Practice
	•	Practice testing
	•	Self-Explanation


	•	My choice of UNIX timeline threads is how Unix and mac connected  through time.




Chapter 1 & Class note summary


	•	Understanding how Operating system works is through abstraction. Which is ignoring detail things and getting on with the point. An example will be if you’re the drive you will not think about what’s in the car rather you’ll be thinking about how to drive it and that’s how abstraction works. Abstraction in Linux consists of three things which is user processes, Linux kernel, and hardware. The User Processes has graphical user, servers, and shell. Also, the user mode restricts access to a subnet of memory and safe CPU operations. The user. 

	•	The 15 commands I learned was :

	•	Cd
	•	Cp
	•	Echo
	•	Kill
	•	More
	•	Mkdir
	•	Mv
	•	Nice
	•	Passwd
10.diff
11. pwd
12.chmod
13. man
14. ps
15. rm




### journal 2


What is /bin?
•	It is a ready to run programs including most of the basic Unix commands such as ls and cp. Also. Most of the programs in /bin are in binary format and is created by C compiler

What does /bin do?
•	/bin are programs that must be available in order to attain minimal functionality for the purposes of starting and repairing a system.

How do you use /bin? 
•	You use it or view it by entering ls /bin in the terminal for my MacBook.



What is /sbin?
•	sbin is a standard subdirectory of the root directory in Linux and other Unix-like operating systems that contains executable ready to run programs. They are mostly administrative tools, that should be made available only to the root for the administrative user.


What does /sbin do?
•	It holds commands needed to boot the system, which are usually not executed by normal users.




How do you use /sbin?
•	A complete list of the contents of /sbin on any system can be seen by using the ls command, which is used to list the contents of directories


What is /usr /bin?
•	/usr/bin is one of the major subdirectories of the /usr directory. /usr, in turn, is one of the largest (in terms of disk space consumption) of the standard first tier directories in the root directory

What does /usr /bin do?
•	This is the primary directory for executable programs. Most programs executed by normal users which are not needed for     booting or for repairing the system and which are not    installed locally should be placed in this directory.

How do you use/usr /bin? 
•	It's an equivalent of the command and generally you use it in scripts in conditional expressions.



What is /usr /sbin?
•	The /usr/sbin directory contains non-vital system utilities that are used after booting (i.e., starting the system) by the system administrator.

What does /usr /sbin do?
•	/usr/sbin also contains some daemons, which are programs that run silently in the background, rather than under the direct control of a user, waiting until they are activated by a particular event or condition. Among the daemons in /usr/sbin are crond, pppd, sshd and xinetd.

How do you use /usr /sbin?
•	/usr/sbin is a subdirectory of /usr, which is used to store many application programs. Another subdirectory of /usr, /usr/bin, contains programs that are not required for booting or repairing the system. The directory /usr/local/sbin is used for locally installed system administration programs.








5 examples of /bin:
1.	cp
2.	pwd
3.	date
4.	sync
5.	ls


5 examples of /sbin:
1.	reboot
2.	ifconfig
3.	route
4.	mount
5.	mknod


5 examples of /usr /bin:
1.	link
2.	ps
3.	bash
4.	cat
5.	sleep


5 examples of /usr /sbin:
1.	/usr : bin, include, local
2.	mount_cd9660
3.	dynamic_pager
4.	md5
5.	nologin


## journal 3

1.	mkdir – make directories
Usage: mkdir [OPTION] DIRECTORY...
eg. mkdir prabhat

2.	ls – list directory contents
Usage: ls [OPTION]... [FILE]... 
eg. ls, ls ­l, ls prabhat

3.	cd – changes directories Usage: 
             cd [DIRECTORY] 
              eg. cd prabhat

4.	pwd - print name of current working directory 
Usage: pwd

5.	cp – copy files and directories
Usage: cp [OPTION]... SOURCE DEST eg. cp sample.txt sample_copy.txt
cp sample_copy.txt target_dir

6.	mv – move (rename) files
Usage: mv [OPTION]... SOURCE DEST eg. mv source.txt target_dir
mv old.txt new.txt

7.	rm ­ remove files or directories 
Usage: rm [OPTION]... FILE...
eg. rm file1.txt , rm ­rf some_dir

8.	cat – concatenate files and print on the standard output 
Usage: cat [OPTION] [FILE]...
eg. cat file1.txt file2.txt

9.	echo – display a line of text
Usage: echo [OPTION] [string] ... 
eg. echo I love India echo $HOME

10.	grep ­ print lines matching a pattern
Usage: grep [OPTION] PATTERN [FILE]... 
eg. grep ­i apple sample.txt


11.	su – change user ID or become super­user 
Usage: su [OPTION] [LOGIN]
eg. su remo, su


###  journal 4


1.	mkdir – make directories
Usage: mkdir [OPTION] DIRECTORY...
eg. mkdir prabhat

2.	ls – list directory contents
Usage: ls [OPTION]... [FILE]... 
eg. ls, ls ­l, ls prabhat

3.	cd – changes directories Usage: 
             cd [DIRECTORY] 
              eg. cd prabhat

4.	pwd - print name of current working directory 
Usage: pwd

5.	cp – copy files and directories
Usage: cp [OPTION]... SOURCE DEST eg. cp sample.txt sample_copy.txt
cp sample_copy.txt target_dir

6.	mv – move (rename) files
Usage: mv [OPTION]... SOURCE DEST eg. mv source.txt target_dir
mv old.txt new.txt

7.	rm ­ remove files or directories 
Usage: rm [OPTION]... FILE...
eg. rm file1.txt , rm ­rf some_dir

8.	cat – concatenate files and print on the standard output 
Usage: cat [OPTION] [FILE]...
eg. cat file1.txt file2.txt

9.	echo – display a line of text
Usage: echo [OPTION] [string] ... 
eg. echo I love India echo $HOME

10.	grep ­ print lines matching a pattern
Usage: grep [OPTION] PATTERN [FILE]... 
eg. grep ­i apple sample.txt


11.	su – change user ID or become super­user 
Usage: su [OPTION] [LOGIN]
eg. su remo, su







### journal 5

-	$ Mkfs: is used to build a Linux filesystem on a device,
(e.g. /dev/hda1, /dev/sdb2),



-	$ mount: mount a filesystem
e.g : mount /dir, mount --target /mountpoint, and mount -t type device dir


-	# fsck: check and repair a Linux filesystem
e.g: fsck [-lsAVRTMNP] [-r [fd]] [-C [fd]] [-t fstype] 


-	$ free: Display amount of free and used memory in the system
e.g: total, used, and free etc…


-	$ ls – list directory contents
Usage: ls [OPTION]... [FILE]... 
eg. ls, ls ­l, ls prabhat


-	$ cd – changes directories Usage: 
             cd [DIRECTORY] 
              eg. cd prabhat


-	$ cat – concatenate files and print on the standard output 
Usage: cat [OPTION] [FILE]...
eg. cat file1.txt file2.txt

-	$ echo – display a line of text
Usage: echo [OPTION] [string] ... 
eg. echo I love India echo $HOME

-	$ grep ­ print lines matching a pattern
Usage: grep [OPTION] PATTERN [FILE]... 
eg. grep ­i apple sample.txt










###  journal 6

-	$ Mkfs: is used to build a Linux filesystem on a device,
(e.g. /dev/hda1, /dev/sdb2),



-	$ mount: mount a filesystem
e.g : mount /dir, mount --target /mountpoint, and mount -t type device dir


-	# fsck: check and repair a Linux filesystem
e.g: fsck [-lsAVRTMNP] [-r [fd]] [-C [fd]] [-t fstype] 


-	$ free: Display amount of free and used memory in the system
e.g: total, used, and free etc…


-	$ ls – list directory contents
Usage: ls [OPTION]... [FILE]... 
eg. ls, ls ­l, ls prabhat


-	$ cd – changes directories Usage: 
             cd [DIRECTORY] 
              eg. cd prabhat


-	$ cat – concatenate files and print on the standard output 
Usage: cat [OPTION] [FILE]...
eg. cat file1.txt file2.txt

-	$ echo – display a line of text
Usage: echo [OPTION] [string] ... 
eg. echo I love India echo $HOME

-	$ grep ­ print lines matching a pattern
Usage: grep [OPTION] PATTERN [FILE]... 
eg. grep ­i apple sample.txt
