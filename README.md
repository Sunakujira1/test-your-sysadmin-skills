<p align="center">
    <img src="https://github.com/trimstray/sysadmin-interview-questions/blob/master/doc/img/sysadmin_interview_questions_preview.png"
        alt="Master">
</p>

<br>

<h4 align="center">Sysadmin Interview Questions 2018 Edition (work in progress).</h4>

<br>

<p align="center">
  <a href="https://github.com/trimstray/sysadmin-interview-questions/tree/master">
    <img src="https://img.shields.io/badge/Branch-master-green.svg?longCache=true"
        alt="Branch">
  </a>
  <a href="http://www.gnu.org/licenses/">
    <img src="https://img.shields.io/badge/License-GNU-blue.svg?longCache=true"
        alt="License">
  </a>
</p>

<div align="center">
  <sub>Created by
  <a href="https://twitter.com/trimstray">trimstray</a> and
  <a href="https://github.com/trimstray/sysadmin-interview-questions/graphs/contributors">
    contributors
  </a>
</div>

<br>

****

## Table of Contents

- <b>[General Knowledge](#general-knowledge)</b>
  * [Junior Sysadmin](#junior-sysadmin) - 30 questions.
  * [Regular Sysadmin](#regular-sysadmin) - 41 questions.
  * [Senior Sysadmin](#senior-sysadmin) - 40 questions.
- <b>[Secret Knowledge](#secret-knowledge)</b>
  * [Guru Sysadmin](#guru-sysadmin) - 7 questions.

## <a name="general-knowledge">General Knowledge</a>

### :diamond_shape_with_a_dot_inside: <a name="junior-sysadmin">Junior Sysadmin</a>

###### System Questions

<details>
<summary><b>What are the Linux Distribution names?</b></summary><br>

- Redhat Enterprise Linux<br>
- Fedora Linux<br>
- CentOS Linux<br>
- Debian Linux<br>
- Ubuntu Linux<br>
- Suse Enterprise Linux<br>
- Slackware Linux

</details>

<details>
<summary><b>What is the difference between Linux and UNIX?</b></summary><br>

UNIX - Only big companies are allowed to use the UNIX copyright and name. IBM AIX, Sun Solaris, and HP-UX all are UNIX operating systems. Most UNIX operating systems are commercial in nature.<br>

- UNIX operating systems are considered as a complete OS as everything come from a single vendor.<br>
- Most UNIX like operating systems are not free.<br>
- UNIX operating systems comes with its own firewall products.<br>
- UNIX supports file systems like jfs, gpfs (AIX), jfs, gpfs (HP-UX), jfs, gpfs (Solaris).<br>

Linux is a Unix clone. But if you consider Portable Operating System Interface (POSIX) standards then Linux can be considered as UNIX.<br>

- Linux is Free. You can download it from the Internet or redistribute it under GNU licenses.<br>
- All Linux distributions include GUI system, GNU utilities, installation & management tools, GNU c/c++ Compilers, Editors (vi), and various applications like OpenOffice, Firefox.<br>
- Linux comes with open source Netfilter and IPTables based firewall tool to protect your server and desktop from the crackers and hackers.<br>
- By default, Linux supports and use ext3 or ext4 file systems.

</details>

<details>
<summary><b>What are some common things between Linux and UNIX?</b></summary><br>

- GUI, file, and windows managers (KDE, Gnome)<br>
- Shells (ksh, csh, bash)<br>
- Various office applications such as OpenOffice.org<br>
- Development tools like perl, php, python, GNU c/c++ compilers<br>
- Posix interface<br>

</details>

<details>
<summary><b>What is Linux and also explain the basic components of this?</b></summary><br>

Linux operating system is consist of 3 components which are as below:<br>

- <b>Kernel</b>: Linux is a monolithic kernel that is free and open source <br>software that is responsible for managing hardware resources for the users.
- <b>System Library</b>: System Library plays a vital role because application programs access Kernels feature using system library.<br>
- <b>System Utility</b>: System Utility performs specific and individual level tasks.

</details>

<details>
<summary><b>What do you understand by CLI?</b></summary><br>

CLI is an acronym for Command Line Interface. We have to provide the information to the computer so that it can perform the function accordingly. In Linux, CLI is the interface that provides the user an interface so that user can type the commands and it complete the tasks. CLI is very easy to use, but it should be typed very precisely.

</details>

<details>
<summary><b>What is your favourite shell and why?</b></summary><br>

BASH as my favorite. It’s really a preferential kind of thing, where I love the syntax and it just "clicks" for me. The input/output redirection syntax (<code>>></code>, <code><< 2>&1</code>, <code>2></code>, <code>1></code>, etc) is similar to C++ which makes it click even easier in my mind.<br>

I also like ZSH shell because is much much more customizable than BASH. It has great Oh-My-Zsh framework, powerful context based tab completion, pattern matching/globbing on alien steroids, loadable modules and more.

</details>

<details>
<summary><b>What is the user ID?</b></summary><br>

Also called login name, logon name, sign-in name, sign-on name. a unique sequence of characters used to identify a user and allow access to a computer system, computer network, or online account. the part of an email address before the @ sign.

</details>

<details>
<summary><b>Describe the root account in Unix-like systems.</b></summary><br>

The root account is like a systems administrator account, and allows you full control of the system. Root always has a UID of zero.

</details>

<details>
<summary><b>How do you find who is logged in?</b></summary><br>

Use this command to find who logged in: <code>w</code>.

</details>

<details>
<summary><b>What is the UID and GID?</b></summary><br>

Unix-like operating systems identify a user within the kernel by a value called a user identifier, often abbreviated to user ID or UID. The UID, along with the group identifier (GID) and other access control criteria, is used to determine which system resources a user can access.

</details>

<details>
<summary><b>Which command is used to review boot messages?</b></summary><br>

<code>dmesg</code> command is used to review boot messages. This command will display system messages contained in the kernel ring buffer. We can use this command immediately after booting to see boot messages. A ring buffer is a buffer of fixed size for which any new data added to it overwrites the oldest data in it.

</details>

<details>
<summary><b>What is the swap space?</b></summary><br>

Swap space is used when the amount of physical memory (RAM) is full. If the system needs more memory resources and the RAM is full, inactive pages in memory are moved to the swap space. While swap space can help machines with a small amount of RAM, it should not be considered a replacement for more RAM. Swap space is located on hard drives, which have a slower access time than physical memory.

</details>

<details>
<summary><b>How to check memory stats and CPU stats?</b></summary><br>

Using <code>free</code> and <code>vmstat</code> command we can display the physical and virtual memory statistics respectively. With the help of <code>sar</code> command we see the CPU utilization & other stats.

</details>

<details>
<summary><b>What is load average?</b></summary><br>

Is the average system load calculated over a given period of time of 1, 5 and 15 minutes. Lower numbers are better. Higher numbers represent a problem or an overloaded machine.

</details>

<details>
<summary><b>How to create partition and filesystem?</b></summary><br>

1) <code>fdisk</code> or <code>gparted</code> - create a new partition<br>
2) <code>mkfs</code> - create a new filesystem

</details>

<details>
<summary><b>Where journaling is dedicated?</b></summary><br>

Journaling has a dedicated area in the file system, where all the changes are tracked. When the system crashes, the possibility of file  system corruption is less because of journaling.

</details>

<details>
<summary><b>What are the kinds of permissions under Unix-like?</b></summary><br>

- <b>Read</b>: users can read the files or list the directory<br>
- <b>Write</b>: users may write to the file or add new files to the directory<br>
- <b>Execute</b>: users may run the file or lookup a specific file within a directory

</details>

<details>
<summary><b>Where is password file located in Linux?</b></summary><br>

Linux passwords are stored in the <b>/etc/shadow</b> file. They are salted and the algorithm being used depends on the particular distribution and is configurable.

</details>

<details>
<summary><b>How do you change directory and subdirectory with file permissions in Linux/UNIX?</b></summary><br>

To change all the directories eg. to 755 (drwxr-xr-x):<br>

<code>
find /opt/data -type d -exec chmod 755 {} \;
</code><br><br>

To change all the files eg. to 644 (-rw-r--r--):<br>

<code>
find /opt/data -type f -exec chmod 644 {} \;
</code><br><br>

</details>

<details>
<summary><b>What is redirection?</b></summary><br>

It’s a fairly simple process, allowing you to direct data from one output to another. You can also use it to direct an output as an input to another process.

</details>

<details>
<summary><b>What is grep command?</b></summary><br>

<code>grep</code> searches file patterns. If you are looking for a specific pattern in the output of another command, grep highlights the relevant lines. Use this grep command for searching log files, specific processes, and more.<br>

</details>

<details>
<summary><b>Explain file content commands along with the description.</b></summary><br>

- <b>head</b>: to check the starting of a file.<br>
- <b>tail</b>: to check the ending of the file. It is the reverse of head command.<br>
- <b>cat</b>: used to view, create, concatenate the files.<br>
- <b>more</b>: used to display the text in the terminal window in pager form.<br>
- <b>less</b>: used to view the text in the backward direction and also provides single line movement.

</details>

<details>
<summary><b>Explain SIGHUP, SIGINT, SIGKILL and SIGTERM Posix signals.</b></summary><br>

- <b>SIGHUP</b> - the SIGHUP signal is sent to a process when its controlling terminal is closed. It was originally designed to notify the process of a serial line drop (a hangup). Many daemons will reload their configuration files and reopen their logfiles instead of exiting when receiving this signal.<br>
- <b>SIGINT</b> - the SIGINT signal is sent to a process by its controlling terminal when a user wishes to interrupt the process. This is typically initiated by pressing Ctrl+C, but on some systems, the "delete" character or "break" key can be used.<br>
- <b>SIGKILL</b> - the SIGKILL signal is sent to a process to cause it to terminate immediately (kill). In contrast to SIGTERM and SIGINT, this signal cannot be caught or ignored, and the receiving process cannot perform any clean-up upon receiving this signal.<br>
- <b>SIGTERM</b> - the SIGTERM signal is sent to a process to request its termination. Unlike the SIGKILL signal, it can be caught and interpreted or ignored by the process. This allows the process to perform nice termination releasing resources and saving state if appropriate. SIGINT is nearly identical to SIGTERM.

</details>

<details>
<summary><b>What is the difference between "rm" and "rm -rf"?</b></summary><br>

<code>rm</code> removes files and <code>-rf</code> are to options:<br>

- <code>-r</code> remove directories and their contents recursively<br>
- <code>-f</code> ignore nonexistent files, never prompt

</details>

<details>
<summary><b>How do you list contents of archive.tgz and extract only one file?</b></summary><br>

<code>
tar tf archive.tgz
</code><br>
<code>
tar xf archive.tgz filename
</code><br>

</details>

<details>
<summary><b>How to sync two local directories?</b></summary><br>

To sync the contents of dir1 to dir2 on the same system, type:

```bash
rsync -av --progress --delete dir1/ dir2
```

- <code>-a, --archive</code> - archive mode
- <code>--delete</code> - delete extraneous files from dest dirs
- <code>-v, --verbose</code> - verbose mode (increase verbosity)
- <code>--progress</code> - show progress during transfer

</details>

###### Network Questions

<details>
<summary><b>What are the default ports used for SMTP, FTP, DNS, DHCP and SSH protocols?</b></summary><br>

<table style="width:100%">
  <tr>
    <th>SERVICE</th>
    <th>PORT</th>
  </tr>
  <tr>
    <td>SMTP</td>
    <td>25</td>
  </tr>
  <tr>
    <td>FTP</td>
    <td>20 for data transfer and 21 for connection established</td>
  </tr>
  <tr>
    <td>DNS</td>
    <td>53</td>
  </tr>
  <tr>
    <td>DHCP</td>
    <td>67/UDP for DHCP server, 68/UDP for DHCP client</td>
  </tr>
  <tr>
    <td>SSH</td>
    <td>22</td>
  </tr>
</table>

</details>

<details>
<summary><b>How to check default route and routing table?</b></summary><br>

Using the commands <code>netstat -nr</code>, <code>route -n</code> or <code>ip route show</code> we can see the default route and routing tables.

</details>

<details>
<summary><b>Why should you avoid telnet to administer a system remotely?</b></summary><br>

Telnet uses most insecure method for communication. It sends data across the network in plain text format and anybody can easily find out the password using the network tool. In the case of Telnet, these include the passing of login credentials in plain text, which means anyone running a sniffer on your network can find the information he needs to take control of a device in a few seconds by eavesdropping on a Telnet login session.

</details>

<details>
<summary><b>What is the difference between wget and curl?</b></summary><br>

The main differences are: wget's major strong side compared to curl is its ability to download recursively. Wget is command line only. Curl supports FTP, FTPS, HTTP, HTTPS, SCP, SFTP, TFTP, TELNET, DICT, LDAP, LDAPS, FILE, POP3, IMAP, SMTP, RTMP and RTSP.

</details>

### :diamond_shape_with_a_dot_inside: <a name="regular-sysadmin">Regular Sysadmin</a>

###### System Questions

<details>
<summary><b>Explain Linux Boot Sequence.</b></summary><br>

<b>BIOS</b>: Full form of BIOS is Basic Input or Output System that performs integrity checks and it will search and load and then it will execute the bootloader.<br>

<b>MBR</b>: MBR means Master Boot Record. MBR contains the information regarding GRUB and executes and loads this bootloader.<br>

<b>GRUB</b>: GRUB means Grand Unified Bootloader. In case, many kernel images are installed on your system then you can select which one you want to execute.<br>

<b>Kernel</b>: Root file system is mounted by Kernel and executes the <code>/sbin/init</code> program.<br>

<b>Init</b>: Init checks the file <code>/etc/inittab</code> and decides the run level. There are seven-run levels available from 0-6. It will identify the default init level and will load the program.<br>

<b>Runlevel programs</b>: As per your default settings for the run level, the system will execute the programs.

</details>

<details>
<summary><b>What is the name and path of the main system log?</b></summary><br>

By default, the main system log is <b>/var/log/messages</b>. This file contains all the messages and the script written by the user.

By default all scripts are saved in this file. This is the standard system log file, which contains messages from all system software, non-kernel boot issues, and messages that go to <code>dmesg</code> (is a system file that is written upon system boot).

</details>

<details>
<summary><b>Explain /proc filesystem.</b></summary><br>

<b>/proc</b> is a virtual file system that provides detailed information about kernel, hardware and running processes.

Since <b>/proc</b> contains virtual files, it is called virtual file system. These virtual files have unique qualities. Most of them are listed as zero bytes in size.<br>

Virtual files such as <b>/proc/interrupts</b>, <b>/proc/meminfo</b>, <b>/proc/mounts</b> and <b>/proc/partitions</b> provide an up-to-the-moment glimpse of the system’s hardware. Others: <b>/proc/filesystems</b> file and the <b>/proc/sys/</b> directory provide system configuration information and interfaces.

</details>

<details>
<summary><b>Why when load is 1.00 on one-core machine is not ideal?</b></summary><br>

The problem with a load of 1.00 is that you have no headroom. In practice, many sysadmins will draw a line at 0.70:<br>

The "Need to Look into it" Rule of Thumb: 0.70 If your load average is staying above > 0.70, it's time to investigate before things get worse.<br>

The "Fix this now" Rule of Thumb: 1.00. If your load average stays above 1.00, find the problem and fix it now. Otherwise, you're going to get woken up in the middle of the night, and it's not going to be fun.<br>

Rule of Thumb: 5.0. If your load average is above 5.00, you could be in serious trouble, your box is either hanging or slowing way down, and this will (inexplicably) happen in the worst possible time like in the middle of the night or when you're presenting at a conference. Don't let it get there.

</details>

<details>
<summary><b>What is umask? How to set it permanently for a user?</b></summary><br>

On Linux and other Unix-like operating systems, new files are created with a default set of permissions. Specifically, a new file's permissions may be restricted in a specific way by applying a permissions "mask" called the umask. The umask command is used to set this mask, or to show you its current value.<br>

Permanently change (set eg. <code>umask 02</code>):<br>

- <b>~/.profile</b><br>
- <b>~/.bashrc</b><br>
- <b>~/.zshrc</b><br>
- <b>~/.cshrc</b>

</details>

<details>
<summary><b>What are symbolic links?</b></summary><br>

A symbolic link, also termed a soft link, is a special kind of file that points to another file, much like a shortcut in Windows or a Macintosh alias. Unlike a hard link, a symbolic link does not contain the data in the target file. It simply points to another entry somewhere in the file system.

</details>

<details>
<summary><b>List out the differences between softlink and hardlink?</b></summary><br>

a) Hardlink cannot be created for directories. Hard link can only be created for a file.<br>

b) Softlink also termed a symbolic links or symlinks can link to a directory.

</details>

<details>
<summary><b>What is the sticky-bit?</b></summary><br>

A Sticky bit is a permission bit that is set on a file or a directory that lets only the owner of the file/directory or the root user to delete or rename the file. No other user is given privileges to delete the file created by some other user.

</details>

<details>
<summary><b>How to change the default run level in Linux?</b></summary><br>

To change the run level we have to edit the file <b>/etc/inittab</b> and change initdefault entry (<code>id:5:initdefault</code>:). Using <code>init</code> command we change the run level temporary like <code>init 3</code>, this command will move the system in runlevl 3.

</details>

<details>
<summary><b>How to add & change the Kernel parameters?</b></summary><br>

To set the kernel parameters in UNIX-like, first edit the file <code>/etc/sysctl.conf</code> after making the changes save the file and run the command <code>sysctl -p</code>, this command will make the changes permanently without rebooting the machine.

</details>

<details>
<summary><b>What is the difference between ext2, ext3 and ext4 file systems?</b></summary>
<br>

<b>ext2</b><br>

- ext2 stands for second extended file system.<br>
- ext2 does not have journaling feature.<br>
- on flash drives, usb drives, ext2 is recommended, as it doesn’t need to do the over head of journaling.<br>
- maximum individual file size can be from 16 GB to 2 TB.<br>
- overall ext2 file system size can be from 2 TB to 32 TB.<br>

<b>ext3</b><br>

- ext3 stands for third extended file system.<br>
- starting from Linux Kernel 2.4.15 ext3 was available.<br>
- the main benefit of ext3 is that it allows journaling.<br>
- maximum individual file size can be from 16 GB to 2 TB.<br>
- overall ext3 file system size can be from 2 TB to 32 TB.<br>
- you can convert a ext2 file system to ext3 file system directly (without backup/restore).<br>

<b>ext4</b><br>

- ext4 stands for fourth extended file system.<br>
- starting from Linux Kernel 2.6.19 ext4 was available.<br>
- supports huge individual file size and overall file system size.<br>
- maximum individual file size can be from 16 GB to 16 TB.<br>
- overall maximum ext4 file system size is 1 EB (exabyte). 1 EB = 1024 PB (petabyte). 1 PB = 1024 TB (terabyte).<br>
- directory can contain a maximum of 64,000 subdirectories (as opposed to 32,000 in ext3).<br>
- you can also mount an existing ext3 fs as ext4 fs (without having to upgrade it).<br>
- several other new features are introduced in ext4: multiblock  allocation, delayed allocation, journal checksum, fast fsck, etc.<br>
- in ext4, you also have the option of turning the journaling feature "off".

</details>

<details>
<summary><b>Explain three types of journaling in ext3/ext4.</b></summary><br>

There are three types of journaling available in ext3/ext4 file systems:

- <b>Journal</b> - metadata and content are saved in the journal.<br>
- <b>Ordered</b> - only metadata is saved in the journal. Metadata are  journaled only after writing the content to disk. This is the default.<br>
- <b>Writeback</b> - only metadata is saved in the journal. Metadata might be  journaled either before or after the content is written to the disk.

</details>

<details>
<summary><b>What is an Inode?</b></summary><br>

An inode is a data structure on a filesystem on Linux and other Unix-like operating systems that stores all the information about a file except its name and its actual data. A data structure is a way of storing data so that it can be used efficiently.<br>

A Unix file is "stored" in two different parts of the disk - the data blocks and the inodes. (I won't get into superblocks and other esoteric information.) The data blocks contain the "contents" of the file. The information about the file is stored elsewhere - in the inode.

</details>

<details>
<summary><b>How to increase the size of LVM partition?</b></summary><br>

Use the <code>lvextend</code> command for resize LVM partition.<br>

- extending the size by 500MB:<br>
<code>
lvextend -L +500M /dev/vgroup/lvolume
</code><br><br>

- extending all available free space:<br>
<code>
lvextend -l +100%FREE /dev/vgroup/lvolume
</code><br><br>

and `resize2fs` or `xfs_growfs` to resize filesystem:<br>

- for ext filesystems:<br>
<code>
resize2fs /dev/vgroup/lvolume
</code><br><br>

- for xfs filesystem:<br>
<code>
xfs_growfs mountpoint_for_/dev/vgroup/lvolume
</code><br><br>

</details>

<details>
<summary><b>Describe a process to create partition, lvm and filesystem.</b></summary><br>

1. Create partition<br>

<code>
fdisk /dev/sdb
</code><br><br>

2. Create LVM<br>

<code>
pvcreate /dev/sdb1
vgcreate vg0 /dev/sdb1
lvcreate --name datastore --size 50G vg0
</code><br><br>

3. Create filesystem<br>

<code>
mkfs -t xfs /dev/mapper/vg0-datastore
</code><br>

</details>

<details>
<summary><b>What is the advantage of executing the running processes in the background? How can you do that?</b></summary><br>

The most significant advantage of executing the running process in the background is that you can do any other task simultaneously while other processes are running in the background. So, more processes can be completed in the background while you are working on different processes. It can be achieved by adding a special character '&' at the end of the command.

</details>

<details>
<summary><b>What is a zombie/defunct process?</b></summary><br>

Is a process that has completed execution (via the <b>exit</b> system call) but still has an entry in the process table: it is a process in the "Terminated state".

</details>

<details>
<summary><b>What if <code>kill -9</code> does not work?</b></summary><br>

<code>kill -9</code> (SIGKILL) always works, provided you have the permission to kill the process. Basically either the process must be started by you and not be setuid or setgid, or you must be root. There is one exception: even root cannot send a fatal signal to PID 1 (the init process).

However <code>kill -9</code> is not guaranteed to work immediately. All signals, including SIGKILL, are delivered asynchronously: the kernel may take its time to deliver them. Usually, delivering a signal takes at most a few microseconds, just the time it takes for the target to get a time slice. However, if the target has blocked the signal, the signal will be queued until the target unblocks it.

Normally, processes cannot block SIGKILL. But kernel code can, and processes execute kernel code when they call system calls.

A process blocked in a system call is in uninterruptible sleep. The <code>ps</code> or <code>top</code> command will (on most unices) show it in state <b>D</b>.

A classical case of long uninterruptible sleep is processes accessing files over NFS when the server is not responding; modern implementations tend not to impose uninterruptible sleep (e.g. under Linux, the intr mount option allows a signal to interrupt NFS file accesses).

You may sometimes see entries marked <b>Z</b> (or <b>H</b> under Linux) in the <code>ps</code> or <code>top</code> output. These are technically not processes, they are zombie processes, which are nothing more than an entry in the process table, kept around so that the parent process can be notified of the death of its child. They will go away when the parent process pays attention (or dies).

</details>

<details>
<summary><b>What is strace command in Linux?</b></summary><br>

strace is a powerful command line tool for debugging and trouble shooting programs in Unix-like operating systems such as Linux. It captures and records all system calls made by a process and the signals received by the process.

</details>

<details>
<summary><b>Which algorithms are supported in passwd file?</b></summary><br>

The algorithms supported are MD5, Blowfish, SHA256 and SHA512.

</details>

<details>
<summary><b>What is key-based authentication? Explain.</b></summary><br>

Key-based authentication is a kind of authentication that may be used as an alternative to password authentication. Instead of requiring a user's password, it is possible to confirm the client's identity by using asymmetric cryptography algorithms, with public and private keys.

</details>

<details>
<summary><b>Which utility is used to make automate rotation of a log?</b></summary><br>

Logrotate command is used to make automate rotation of log. It allows automatic rotation, compression, removal, and mailing of log files.

</details>

<details>
<summary><b>What is the use of ulimit in Unix-like systems?</b></summary><br>

Most UNIX-like operating systems, including Linux and BSD, provide ways to limit and control the usage of system resources such as threads, files, and network connections on a per-process and per-user basis. These "ulimits" prevent single users from using too many system resources.

</details>

<details>
<summary><b>What are soft limits and hard limits?</b></summary><br>

Hard limit is the maximum allowed to a user, set by the superuser or root. This value is set in the file <code>/etc/security/limits.conf</code>. The user can increase the soft limit on their own in times of needing more resources, but cannot set the soft limit higher than the hard limit.

</details>

<details>
<summary><b>What is the difference between Cron and Anacron?</b></summary><br>

- one of the main difference between cron and anacron jobs is that cron works on the system that are running continuously that means it is designed for the system that is running24*7. While anacron is used for the systems that are not running continuously.<br>
- other difference between the two is cron jobs can run every minute, but anacron jobs can be run only once a day.<br>
- any normal user can do the scheduling of cron jobs, but the scheduling of anacron jobs can be done by the superuser only.<br>
- cron should be used when you need to execute the job at a specific time as per the given time in cron, but anacron should be used in when there is no any restriction for the timing and can be executed at any time.

</details>

<details>
<summary><b>Create a file with 100000 lines with random values.</b></summary><br>

For example:

```bash
for i in $(seq 1 100000) ; do
  rand=$(cat /dev/urandom | tr -dc 'a-zA-Z0-9' | fold -w 32 | head -n 1)
  echo "$rand" >> /path/to/file
done
```

</details>

<details>
<summary><b>How to run script as another user without password?</b></summary><br>

For example (with <code>visudo</code> command):

```bash
user1 ALL=(user2) NOPASSWD: /opt/scripts/bin/generate.sh
```

The command paths must be absolute! Then call <code>sudo -u user2 /opt/scripts/bin/generate.sh</code> from a user1 shell.

</details>

<details>
<summary><b>How to check if running as root in a bash script?</b></summary><br>

In a bash script, you have several ways to check if the running user is root.

As a warning, do not check if a user is root by using the root username. Nothing guarantees that the user with ID 0 is called root. It's a very strong convention that is broadly followed but anybody could rename the superuser another name.

I think the best way when using bash is to use $EUID because $UID could be changed and not reflect the real user running the script.

```bash
if (( $EUID != 0 )); then
  echo "Please run as root"
  exit
fi
```
</details>

<details>
<summary><b>How to <code>git clone</code> including submodules?</b></summary><br>

For example:

```bash
# With -j8 - performance optimization
git clone --recurse-submodules -j8 git://github.com/foo/bar.git

# For already cloned repos or older Git versions
git clone git://github.com/foo/bar.git
cd bar
git submodule update --init --recursive
```

</details>

<details>
<summary><b>Is there a way to redirect output to a file and have it display on stdout?</b></summary><br>

The command you want is named tee:

`foo | tee output.file`

For example, if you only care about stdout:

`ls -a | tee output.file`

If you want to include stderr, do:

`program [arguments...] 2>&1 | tee outfile`

`2>&1` redirects channel 2 (stderr/standard error) into channel 1 (stdout/standard output), such that both is written as stdout. It is also directed to the given output file as of the tee command.

Furthermore, if you want to append to the log file, use tee -a as:

`program [arguments...] 2>&1 | tee -a outfile`

</details>

<details>
<summary><b>What is the preferred Bash shebang?</b></summary><br>

You should use <code>#!/usr/bin/env bash</code> for portability: different *nixes put bash in different places, and using <code>/usr/bin/env</code> is a workaround to run the first bash found on the PATH.

</details>

</details>

<details>
<summary><b>How to get fingerprint from SSH key?</b></summary><br>

```
ssh-keygen -lf ~/.ssh/id_rsa.pub
```

</details>

<details>
<summary><b>What is root certificate and intermediate certificate?</b></summary><br>

A "root" authority is a certificate issuer that parties choose to trust (explicitly). It is usually self-signed (self-issued) and very highly protected. An intermediate authority is a certificate issuer that has itself been issued by a root or another higher level intermediate authority.

</details>

<details>
<summary><b>How to reloading PostgreSQL after configuration changes?</b></summary><br>

Solution 1:

```
systemctl reload postgresql
```

Solution 2:

```
su - postgres
/usr/bin/pg_ctl reload
```

Solution 3:

```
SELECT pg_reload_conf();
```

</details>

<details>
<summary><b>How to restore config file in Debian GNU/Linux?</b></summary><br>

Will recreate any missing configuration files, eg. <code>/etc/mysql/my.cnf</code> in your case:

```
dpkg -i --force-confmiss mysql-common.deb
```

</details>

###### Network Questions

<details>
<summary><b>How to check which ports are listening in my Linux Server?</b></summary><br>

Use the <code>netstat -tapn</code> or <code>lsof -i</code>.

</details>

<details>
<summary><b>How to send an HTTP request using Telnet?</b></summary><br>

For example:

```bash
telnet example.com 80
Trying 192.168.252.10...
Connected to example.com.
Escape character is '^]'.
GET /questions HTTP/1.0
Host: example.com

HTTP/1.1 200 OK
Content-Type: text/html; charset=utf-8
...
```

</details>

<details>
<summary><b>How to allow traffic to/from specific IP with iptables?</b></summary><br>

For example:

```bash
/sbin/iptables -A INPUT -p tcp -s XXX.XXX.XXX.XXX -j ACCEPT
/sbin/iptables -A OUTPUT -p tcp -d  XXX.XXX.XXX.XXX -j ACCEPT
```

</details>

<details>
<summary><b>How to block abusive IP addresses with <code>pf</code> in OpenBSD?</b></summary><br>

The best way to do this is to define a table and create a rule to block the hosts, in <code>pf.conf</code>:

```bash
table <badhosts> persist
block on fxp0 from <badhosts> to any
```

And then dynamically add/delete IP addresses from it:

```bash
pfctl -t badhosts -T add 1.2.3.4
pfctl -t badhosts -T delete 1.2.3.4
```

</details>

<details>
<summary><b>How to disable Cache for specific domain in Varnish?</b></summary><br>

For example:

```
sub vcl_recv {
   # dont cache foo.com or bar.com - optional www
   if (req.host ~ "(www)?(foo|bar).com") {
     return(pass);
   }
}
```

or:

```
sub vcl_recv {
  # dont cache foo.com or bar.com - optional www
   if (req.http.host ~ "(www\.)?(foo|bar)\.com") {
     return(pass);
   }
  # cache foobar.com - optional www
   if (req.http.host ~ "(www\.)?foobar\.com") {
     return(hash);
   }
}
```

</details>

<details>
<summary><b>What is the difference between CORS and CSPs?</b></summary><br>

CORS allows the Same Origin Policy to be relaxed for a domain.

e.g. normally if the user logs into both example.com and <code>example.org</code>, the Same Origin Policy prevents <code>example.com</code> from making an AJAX request to <code>example.org/current_user/full_user_details</code> and gaining access to the response.

This is the default policy of the web and prevents the user's data from being leaked when logged into multiple sites at the same time.

Now with CORS, example.org could set a policy to say it will allow the origin <code>https://example.com</code> to read responses made by AJAX. This would be done if both example.com and example.org are ran by the same company and data sharing between the origins is to be allowed in the user's browser. It only affects the client-side of things, not the server-side.

CSPs on the other hand set a policy of what content can run on the current site. For example, if JavaScript can be executed inline, or which domains .js files can be loaded from. This can be beneficial to act as another line of defence against XSS attacks, where the attacker will try and inject script into the HTML page. Normally output would be encoded, however say the developer had forgotten only on one output field. Because the policy is preventing in-line script from executing, the attack is thwarted.

</details>

### :diamond_shape_with_a_dot_inside: <a name="senior-sysadmin">Senior Sysadmin</a>

###### System Questions

<details>
<summary><b>What are the different types of Kernels? Explain.</b></summary><br>

- <b>Microkernel</b>: This type of kernel only manages CPU, memory, and IPC. This kind of kernel provides portability, small memory footprint and also security.<br>
- <b>Monolithic Kernel</b>: Linux is a monolithic kernel. So, this type of kernel provides file management, system server calls, also manages CPU, IPC as well as device drivers. It provides easier access to the process to communicate and as there is not any queue for processor time, so processes react faster.<br>
- <b>Hybrid Kernel</b>: In this type of kernels, programmers can select what they want to run in user mode and what in supervisor mode. So, this kernel provides more flexibility than any other kernel but it can have some latency problems.

</details>

<details>
<summary><b>What is LD_LIBRARY_PATH?</b></summary><br>

Environment variable LD_LIBRARY_PATH is a colon-separated set of directories where libraries should be searched for first, before the standard set of directories; this is useful when debugging a new library or using a nonstandard library for special purposes.

</details>

<details>
<summary><b>How shadow passwords are given by in Linux?</b></summary><br>

<code>pwconv</code> command is used for giving shadow passwords. Shadow passwords are given for better system security. The <code>pwconv</code> command creates the file <code>/etc/shadow</code> and changes all passwords to 'x' in the <code>/etc/passwd</code> file.

</details>

<details>
<summary><b>Explain all the fields in the /etc/passwd file.</b></summary><br>

- <b>Username</b>: First field is the username that contains the username which is 1 to 32 length characters.<br>
- <b>Password</b>: This field does not show the actual password as the password is encrypted. Here, x character shows that password is encrypted that is located in <code>/etc/shadow</code> file.<br>
- <b>User ID (UID)</b>: All the users created in Linux is given a user ID whenever the user is created. UID 0 is fixed and reserved for the root user.<br>
- <b>Group ID (GID)</b>: This field specifies the name of the group to which the user belongs. The group information is also stored in a file <code>/etc/group</code>.<br>
- <b>User ID Info</b>: Here you can add comments and you can add any extra information related to the users like full name, contact number, etc.<br>
- <b>Home directory</b>: This field provides the path where the user is directed after the login. For example, <code>/home/smith</code>.<br>
- <b>Command/shell</b>: This field provides the path of a command/shell and denotes that user has access to this shell i.e. /bin/bash.

</details>

<details>
<summary><b>What does Sar provides and at which location Sar logs are stored?</b></summary><br>

Sar collect, report or save system activity information. The default version of the sar command (CPU utilization report) might be one of the first facilities the user runs to begin system activity investigation, because it monitors major system resources. If CPU utilization is near 100 percent (user + nice + system), the workload sampled is CPU-bound.

By default log files of Sar command is located at <code>/var/log/sa/sadd</code> file, where the dd parameter indicates the current day.

</details>

<details>
<summary><b>How to scan newly assigned luns on linux box without rebooting?</b></summary><br>

Run the command: <code>echo "---" >/sys/class/scsi_host/hostX/scan</code>.

</details>

<details>
<summary><b>Explain system calls used for process management?</b></summary><br>

There are some system calls used in Linux for process management. These are as follows:<br>

- <code>Fork()</code>: It is used to create a new process<br>
- <code>Exec()</code>: It is used to execute a new process<br>
- <code>Wait()</code>: It is used to make the process to wait<br>
- <code>Exit()</code>: It is used to exit or terminate the process<br>
- <code>Getpid()</code>: It is used to find the unique process ID<br>
- <code>Getppid()</code>: It is used to check the parent process ID<br>
- <code>Nice()</code>: It is used to bias the currently running process property

</details>

<details>
<summary><b>Explain interrupts in Linux and also explain interrupt handlers.</b></summary><br>

Interrupts means the processor is transferred temporarily to another program or function. When that program is completed, the processor will be given back to that program to complete the task.

Interrupt handler is the function that the kernel runs for a specific interrupt. It is also called Interrupt Service Routine. Interrupts handlers are the function that matches a particular prototype and enables the kernel to pass the handler information accurately.

</details>

<details>
<summary><b>How can we edit a file without opening in Linux?</b></summary><br>

For example:<br>

```bash
cat >> /path/to/file << __EOF__
How to Use the VI Editor.
__EOF__
```

</details>

<details>
<summary><b>What is the Pluggable Authentication Modules? Explain.</b></summary><br>

It provides a layer between applications and actual authentication mechanism. It is a library of loadable modules which are called by the application for authentication. It also allows the administrator to control when a user can log in. All PAM applications are configured in the directory <code>/etc/pam.d</code> or in a file <code>/etc/pam.conf</code>. PAM is controlled using the configuration file or the configuration directory.

</details>

<details>
<summary><b>How do you run command every time a file is modified?</b></summary><br>

For example:<br>

```bash
while inotifywait -e close_write filename ; do

  echo "changed" >> /var/log/changed

done
```

</details>

<details>
<summary><b>What is the Superblock?</b></summary><br>

A superblock is a record of the characteristics of a filesystem, including its size, the block size, the empty and the filled blocks and their respective counts, the size and location of the inode tables, the disk block map and usage information, and the size of the block groups.

</details>

<details>
<summary><b>What is the use of Suid?</b></summary><br>

An "s" in the first position means that the SETUID (or SUID) bit was set (the GUID bit is the same thing, at the group level). Linux runs an executable file with the SETUID bit set with the User ID (that is, the privileges!) of the owner of that file, not the one of the user who launched it.

</details>

<details>
<summary><b>What does a kill command do?</b></summary><br>

In Unix and Unix-like operating systems, kill is a command used to send a signal to a process. By default, the message sent is the termination signal, which requests that the process exit. But kill is something of a misnomer; the signal sent may have nothing to do with process killing.

</details>

<details>
<summary><b>Describe exceptions for which the use of SIGKILL is insufficient.</b></summary><br>

- Zombie processes cannot be killed since they are already dead and waiting for their parent processes to reap them.<br>
- Processes that are in the blocked state will not die until they wake up again.<br>
- The init process is special: It does not get signals that it does not want to handle, and thus it can ignore SIGKILL. An exception from this exception is while init is ptraced on Linux.<br>
- An uninterruptibly sleeping process may not terminate (and free its resources) even when sent SIGKILL. This is one of the few cases in which a UNIX system may have to be rebooted to solve a temporary software problem.

</details>

<details>
<summary><b>Present and explain the correct process path using the kill command.</b></summary><br>

Speaking of killing processes never use <code>kill -9/SIGKILL</code> unless absolutely mandatory. This kill can cause problems because of its brute force.

Always try to use the following simple procedure:

- first, send <b>SIGTERM</b> (<code>kill -15</code>) signal first which tells the process to shutdown and is generally accepted as the signal to use when shutting down cleanly (but remember that this signal can be ignored).
- next try to send <b>SIGHUP</b> (<code>kill -1</code>) signal which is commonly used to tell a process to shutdown and restart, this signal can also be caught and ignored by a process.

The far majority of the time, this is all you need - and is much cleaner.

</details>

<details>
<summary><b>What was getfacl and setfacl commands do?</b></summary><br>

The command "setfacl" refers to Set File Access Control Lists and "getfacl" refers to Get File Access Control List. Each file and directory in a Linux filesystem is created with a specific set of file permissions for its access. In order to know the access permissions of a file or directory we use getfacl.

</details>

<details>
<summary><b>What is a file descriptor in Linux?</b></summary><br>

In Unix and related computer operating systems, a file descriptor (FD, less frequently fildes) is an abstract indicator (handle) used to access a file or other input/output resource, such as a pipe or network socket. File descriptors form part of the POSIX application programming interface.

</details>

<details>
<summary><b>What is an open file table?</b></summary><br>

The process table entry (aka process control block) contains a table, the file descriptor table that gives the mapping between the descriptor the process uses to refer to a file connection and the data structure inside the kernel that represents the actual file connection.

</details>

<details>
<summary><b>What's the difference between /sbin/nologin, /bin/false and /bin/true?
</b></summary><br>

When <code>/sbin/nologin</code> is set as the shell, if user with that shell logs in, they'll get a polite message saying 'This account is currently not available.'

<code>/bin/false</code> is just a binary that immediately exits, returning false, when it's called, so when someone who has false as shell logs in, they're immediately logged out when false exits. Setting the shell to <code>/bin/true</code> has the same effect of not allowing someone to log in but false is probably used as a convention over true since it's much better at conveying the concept that person doesn't have a shell.

nologin is the more user-friendly option, with a customizable message given to the user trying to log in, so you would theoretically want to use that; but both nologin and false will have the same end result of someone not having a shell and not being able to ssh in.

</details>

<details>
<summary><b>How to read a file line by line and assigning the value to a variable.</b></summary><br>

For example:

```bash
while IFS='' read -r line || [[ -n "$line" ]] ; do
  echo "Text read from file: $line"
done < "/path/to/filename"
```

Explanation:

- <code>IFS=''</code> (or <code>IFS=</code>) prevents leading/trailing whitespace from being trimmed.
- <code>-r</code> prevents backslash escapes from being interpreted.
- <code>|| [[ -n $line ]]</code> prevents the last line from being ignored if it doesn't end with a <code>\n</code> (since  read returns a non-zero exit code when it encounters EOF).

</details>

<details>
<summary><b>How to rebuild Initial Ramdisk Image in Debian/CentOS?</b></summary><br>

Debian GNU/Linux:

```bash
update-initramfs -m -k all
update-grub
```

CentOS Linux:

```bash
dracut -f
grub2-mkconfig -o /boot/grub/grub.cfg
```

</details>

<details>
<summary><b>What does "CPU jumps" mean?</b></summary><br>

An OS is a very busy thing, particularly so when you have it doing something (and even when you aren't). And when we are looking at an active enterprise environment, something is always going on.

Most of this activity is "bursty", meaning processes are typically quiescent with short periods of intense activity. This is certainly true of any type of network-based activity (e.g. processing PHP requests), but also applies to OS maintenance (e.g. file system maintenance, page reclamation, disk I/O requests).

If you take a situation where you have a lot of such bursty processes, you get a very irregular and spiky CPU usage plot.

As "500 - Internal Server Error" says, the high number of context switches are going to make the situation even worse.

</details>

<details>
<summary><b>How does strace connect to an already running process?</b></summary><br>

`strace -p <PID>` - to attach a process to strace.

`strace -e trace=read,write -p <PID>` - by this you can also trace a process/program for an event, like read and write (in this example). So here it will print all such events that include read and write system calls by the process.

Other such examples

- `-e trace= network` - trace all the network related system calls.
- `-e trace=signal` - trace all signal related system calls.
- `-e trace=ipc` - trace all IPC related system calls.
- `-e trace=desc` - trace all file descriptor related system calls.
- `-e trace=memory` - trace all memory mapping related system calls.

</details>

<details>
<summary><b>How to remove all files except some from a directory?</b></summary><br>

Solution 1 - with <b>extglob</b>:

```
shopt -s extglob
rm !(textfile.txt|backup.tar.gz|script.php|database.sql|info.txt)
```

Solution 2 - with <b>find</b>:

```
find . -type f -not -name '*txt' -print0 | xargs -0 rm --
```

</details>

<details>
<summary><b>How to check if a string contains a substring in Bash?</b></summary><br>

You can use * (wildcards) outside a case statement, too, if you use double brackets:

```bash
string='some text'
if [[ $string = *"My long"* ]] ; then
  true
fi
```

</details>

<details>
<summary><b>How to redirect stderr and stdout to different files in the same line?</b></summary><br>

Just add them in one line <code>command 2>> error 1>> output</code>.

However, note that <code>>></code> is for appending if the file already has data. Whereas, <code>></code> will overwrite any existing data in the file.

So, <code>command 2> error 1> output</code> if you do not want to append.

Just for completion's sake, you can write <code>1></code> as just <code>></code> since the default file descriptor is the output. so <code>1></code> and <code>></code> is the same thing.

So, <code>command 2> error 1> output</code> becomes, <code>command 2> error > output</code>.

</details>

<details>
<summary><b>How to remove leading whitespace from each line in a file?</b></summary><br>

Warning: this will overwrite the original file:

```bash
sed -i "s/^[ \t]*//" filename
```

or:

```bash
sed 's/^[ \t]+//g' < input > output
```

</details>

<details>
<summary><b>Getting Too many Open files error for Postgres. How to resolve it?</b></summary><br>

Fixed the issue by reducing <code>max_files_per_process</code> eg. to 200 from default 1000. This parameter is in <code>postgresql.conf</code> file and this sets the maximum number of simultaneously open files allowed to each server subprocess.

Usually people start to edit <code>/etc/security/limits.conf</code> file, but forget that this file only apply to the actively logged in users through the pam system.

</details>

<details>
<summary><b>How to log all commands run by root on production servers?</b></summary><br>

<code>auditd</code> is the correct tool for the job here:

1. Add these 2 lines to <code>/etc/audit/audit.rules</code>:

```bash
-a exit,always -F arch=b64 -F euid=0 -S execve
-a exit,always -F arch=b32 -F euid=0 -S execve
```

These will track all commands run by root (euid=0). Why two rules? The execve syscall must be tracked in both 32 and 64 bit code.

2. To get rid of auid=4294967295 messages in logs, add audit=1 to the kernel's cmdline (by editing <code>/etc/default/grub</code>)

3. Place the line

```bash
session  required                pam_loginuid.so
```

in all PAM config files that are relevant to login (<code>/etc/pam.d/{login,kdm,sshd}</code>), but not in the files that are relevant to su or sudo. This will allow auditd to get the calling user's uid correctly when calling sudo or su.

Restart your system now.

Let's login and run some commands:

```bash
$ id -u
1000
$ sudo ls /
bin  boot  data  dev  etc  home  initrd.img  initrd.img.old  lib  lib32  lib64  lost+found  media  mnt  opt  proc  root  run  sbin  scratch  selinux  srv  sys  tmp  usr  var  vmlinuz  vmlinuz.old
$ sudo su -
# ls /etc
[...]
```

Now read <code>/var/log/audit/auditd.log</code> for show what has been logged in.

</details>

<details>
<summary><b>How to prevent <code>dd</code> from freezing system?</b></summary><br>

Try using ionice:

```bash
ionice -c3 dd if=/dev/zero of=z
```

This start the <code>dd</code> process with the "idle" IO priority: it only gets disk time when no other process is using disk IO for a certain amount of time.

Of course this can still flood the buffer cache and cause freezes while the system flushes out the cache to disk. There are tunables under <code>/proc/sys/vm/</code> to influence this, particularly the dirty_* entries.

</details>

<details>
<summary><b>How to limiting processes to not exceed more than X% of CPU usage?</b></summary><br>

- <b>nice/renice</b>

nice is a great tool for 'one off' tweaks to a system:

`nice COMMAND`

- <b>cpulimit</b>

cpulimit if you need to run a CPU intensive job and having free CPU time is essential for the responsiveness of a system:

`cpulimit -l 50 COMMAND`

- <b>cgroups</b>

cgroups apply limits to a set of processes, rather than to just one:

```
cgcreate -g cpu:/cpulimited
cgset -r cpu.shares=512 cpulimited
cgexec -g cpu:cpulimited COMMAND_1
cgexec -g cpu:cpulimited COMMAND_2
cgexec -g cpu:cpulimited COMMAND_3
```

</details>

###### Network Questions

<details>
<summary><b>How do you kill program using one port in Linux?</b></summary><br>

To list any process listening to the port 8080:<br>

<code>lsof -i:8080</code>

To kill any process listening to the port 8080:<br>

<code>kill $(lsof -t -i:8080)</code>

or more violently:<br>

<code>kill -9 $(lsof -t -i:8080)</code><br><br>

</details>

<details>
<summary><b>How to testing connection to remote host (with and without SNI)?</b></summary><br>

With <b>OpenSSL</b>:

```bash
# Testing connection to remote host (with SNI support)
echo | openssl s_client -showcerts -servername google.com -connect google.com:443
# Testing connection to remote host (without SNI support)
echo | openssl s_client -connect google.com:443 -showcerts
```

With <b>GnuTLS</b>:

```bash
# Testing connection to remote host (with SNI support)
gnutls-cli -p 443 google.com
# Testing connection to remote host (without SNI support)
gnutls-cli --disable-sni -p 443 google.com
```

</details>

<details>
<summary><b>How are cookies passed in the HTTP protocol?</b></summary><br>

The server sends the following in its response header to set a cookie field:

`Set-Cookie:name=value`

If there is a cookie set, then the browser sends the following in its request header:

`Cookie:name=value`

</details>

<details>
<summary><b>What is the proper way to test NFS performance?
</b></summary><br>

The best benchmark is always "the application(s) that you normally use". The load on a NFS system when you have 20 people simultaneously compiling a Linux kernel is comletely different from a bunch of people logging in at the same time or the accounts uses as "home directories for the local web-server".

But we have some good tools for testing this.

- <b>boonie</b> - a classical performances evaluation tool tests. The main program tests database type access to a single file (or a set of files if you wish to test more than 1G of storage), and it tests creation, reading, and deleting of small files which can simulate the usage of programs such as Squid, INN, or Maildir format email.
- <b>DBench</b> - was written to allow independent developers to debug and test SAMBA. It is heavily inspired of the original SAMBA tool.
- <b>IOZone</b> - performance tests suite. POSIX and 64 bits compliant. This tests is the file system test from the L.S.E. Main features: POSIX async I/O, Mmap() file I/O, Normal file I/O Single stream measurement, Multiple stream measurement, Distributed file server measurements (Cluster) POSIX pthreads, Multi-process measurement Selectable measurements with fsync, O_SYNC Latency plots.

</details>

<details>
<summary><b>How to run scp with a second remote host?</b></summary><br>

With <b>ssh</b>:

```
ssh user1@remote1 'ssh user2@remote2 "cat file"' > file
```

With <b>tar</b> (with compression):

```
ssh user1@remote1 'ssh user2@remote2 "cd path2; tar cj file"' | tar xj
```

With <b>ssh</b> and port forwarding tunnel:

```
# First, open the tunnel
ssh -L 1234:remote2:22 -p 45678 user1@remote1
# Then, use the tunnel to copy the file directly from remote2
scp -P 1234 user2@localhost:file .
```

</details>

<details>
<summary><b>Explain difference between HTTP 1.1 and HTTP 2.0.</b></summary><br>

<b>HTTP/2</b> supports queries multiplexing, headers compression, priority and more intelligent packet streaming management. This results in reduced latency and accelerates content download on modern web pages.

Key differences with HTTP/1.1:

- it is binary, instead of textual
- fully multiplexed, instead of ordered and blocking
- can therefore use one connection for parallelism
- uses header compression to reduce overhead
- allows servers to “push” responses proactively into client caches

</details>

<details>
<summary><b>What's the difference between <code>Cache-Control: max-age=0</code> and <code>no-cache</code>?</b></summary><br>

When sent by the origin server:

<code>max-age=0</code> simply tells caches (and user agents) the response is stale from the get-go and so they SHOULD revalidate the response (eg. with the If-Not-Modified header) before using a cached copy, whereas, <code>no-cache</code> tells them they MUST revalidate before using a cached copy.

In other words, caches may sometimes choose to use a stale response (although I believe they have to then add a Warning header), but <code>no-cache</code> says they're not allowed to use a stale response no matter what. Maybe you'd want the SHOULD-revalidate behavior when baseball stats are generated in a page, but you'd want the MUST-revalidate behavior when you've generated the response to an e-commerce purchase.

When sent by the user agent:

If a user agent sends a request with <code>Cache-Control: max-age=0</code> (aka. "end-to-end revalidation"), then each cache along the way will revalidate its cache entry (eg. with the If-Not-Modified header) all the way to the origin server. If the reply is then 304 (Not Modified), the cached entity can be used.

On the other hand, sending a request with <code>Cache-Control: no-cache</code> (aka. "end-to-end reload") doesn't revalidate and the server MUST NOT use a cached copy when responding.

</details>

<details>
<summary><b>What are the security risks of setting <code>Access-Control-Allow-Origin</code>?</b></summary><br>

By responding with <code>Access-Control-Allow-Origin: *</code>, the requested resource allows sharing with every origin. This basically means that any site can send an XHR request to your site and access the server’s response which would not be the case if you hadn’t implemented this CORS response.

So any site can make a request to your site on behalf of their visitors and process its response. If you have something implemented like an authentication or authorization scheme that is based on something that is automatically provided by the browser (cookies, cookie-based sessions, etc.), the requests triggered by the third party sites will use them too.

</details>

## <a name="secret-knowledge">Secret Knowledge</a>

### :diamond_shape_with_a_dot_inside: Guru Sysadmin

3 Questions.

<details>
<summary><b>Why do We need mktemp command?</b></summary><br>

<code>mktemp</code> randomizes the name. It is very important from the security point of view.

Just imagine that you do something like:

```bash
echo "random_string" > /tmp/temp-file
```

in your root-running script. And someone (who has read your script) does

```bash
ln -s /etc/passwd /tmp/temp-file
```

The <code>mktemp</code> command could help you in this situation:

```bash
TEMP=$(mktemp /tmp/temp-file.XXXXXXXX)
echo "random_string" > ${TEMP}
```

Now this <code>ln /etc/passwd</code> attack will not work.

</details>

<details>
<summary><b>Use sysfs virtual filesystem to testing connection on all interfaces (without loopback).</b></summary><br>

For example:

```bash
#!/usr/bin/bash

for iface in $(ls /sys/class/net/ | grep -v lo) ; do

  if [[ $(cat /sys/class/net/$iface/carrier) = 1 ]] ; then state=1 ; fi

done

if [[ $state -ne 0 ]] ; then echo "not connection" > /dev/stderr ; exit ; fi
```

</details>

<details>
<summary><b>Explain Varnish Cache SHM Log (pooling mechanism).</b></summary><br>

Every poll is recorded in the shared memory log as follows:

```
0 Backend_health - b0 Still healthy 4--X-S-RH 9 8 10 0.029291 0.030875 HTTP/1.1 200 Ok
```

The fields are:

- 0 - Constant
- Backend_health - Log record tag
- '-' client/backend indication (XXX: wrong! should be 'b')
- b0 - Name of backend (XXX: needs qualifier)
- two words indicating state:
  - "Still healthy"
  - "Still sick"
  - "Back healthy"
  - "Went sick"

Notice that the second word indicates present state, and the first word == "Still" indicates unchanged state.

- 4--X-S-RH - Flags indicating how the latest poll went
  - 4 - IPv4 connection established
  - 6 - IPv6 connection established
  - x - Request transmit failed
  - X - Request transmit succeeded
  - s - TCP socket shutdown failed
  - S - TCP socket shutdown succeeded
  - r - Read response failed
  - R - Read response succeeded
  - H - Happy with result
- 9 - Number of good polls in the last .window polls
- 8 - .threshold (see above)
- 10 - .window (see above)
- 0.029291 - Response time this poll or zero if it failed
- 0.030875 - Exponential average (r=4) of responsetime for good polls.
- HTTP/1.1 200 Ok - The HTTP response from the backend.

</details>

<details>
<summary><b>How to rewrite POST data with Payload in Nginx?</b></summary><br>

You just need to write a Nginx rewrite rule with HTTP status code <b>307</b> or <b>308</b>:

```bash
location ~ ^/de/api/(?<method>.*)$ {
    if ($request_method = POST) {
        return 307 http://www.example.com/api/$method$is_args$args;
    }

    # You can keep this for non-POST requests
    rewrite ^/de/api/(.*) http://www.example.com/api/$1 redirect;
}
```

HTTP Status code 307 or 308 should be used instead of 301 because it changes the request method from POST to GET.

</details>

<details>
<summary><b>Should the root certificate go on the server?</b></summary><br>

Self-signed root certificates need not/should not be included in web server configuration. They serve no purpose (clients will always ignore them) and they incur a slight performance (latency) penalty because they increase the size of the SSL handshake.

If the client does not have the root in their trust store, then it won't trust the web site, and there is no way to work around that problem. Having the web server send the root certificate will not help - the root certificate has to come from a trusted 3rd party (in most cases the browser vendor).

</details>

<details>
<summary><b>How do I measure request and response times at once using cURL?</b></summary><br>

cURL supports formatted output for the details of the request (see the cURL manpage for details, under <code>-w| -write-out 'format'</code>). For our purposes we’ll focus just on the timing details that are provided.

1. Create a new file, curl-format.txt, and paste in:

```bash
    time_namelookup:  %{time_namelookup}\n
       time_connect:  %{time_connect}\n
    time_appconnect:  %{time_appconnect}\n
   time_pretransfer:  %{time_pretransfer}\n
      time_redirect:  %{time_redirect}\n
 time_starttransfer:  %{time_starttransfer}\n
                    ----------\n
         time_total:  %{time_total}\n
```

2. Make a request:

```
curl -w "@curl-format.txt" -o /dev/null -s "http://example.com/"
```

What this does:

- <code>-w "@curl-format.txt"</code> - tells cURL to use our format file
- <code>-o /dev/null</code> - redirects the output of the request to /dev/null
- <code>-s</code> - tells cURL not to show a progress meter
<code>http://example.com/</code> is the URL we are requesting. Use quotes particularly if your URL has "&" query string parameters

</details>

<details>
<summary><b>Is there a way to allow multiple cross-domains using the Access-Control-Allow-Origin header in Nginx?</b></summary><br>

For Nginx users to allow CORS for multiple domains. To match a list of domain and subdomain this regex make it ease to work with fonts:

```
location ~* \.(?:ttf|ttc|otf|eot|woff|woff2)$ {
   if ( $http_origin ~* (https?://(.+\.)?(domain1|domain2|domain3)\.(?:me|co|com)$) ) {
      add_header "Access-Control-Allow-Origin" "$http_origin";
   }
}
```

More sligtly configuration:

```
location / {

    if ($http_origin ~* (^https?://([^/]+\.)*(domainone|domaintwo)\.com$)) {
        set $cors "true";
    }

    # Nginx doesn't support nested If statements. This is where things get slightly nasty.
    # Determine the HTTP request method used
    if ($request_method = 'GET') {
        set $cors "${cors}get";
    }
    if ($request_method = 'POST') {
        set $cors "${cors}post";
    }

    if ($cors = "true") {
        # Catch all incase there's a request method we're not dealing with properly
        add_header 'Access-Control-Allow-Origin' "$http_origin";
    }

    if ($cors = "trueget") {
        add_header 'Access-Control-Allow-Origin' "$http_origin";
        add_header 'Access-Control-Allow-Credentials' 'true';
        add_header 'Access-Control-Allow-Methods' 'GET, POST, OPTIONS';
        add_header 'Access-Control-Allow-Headers' 'DNT,X-CustomHeader,Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type';
    }

    if ($cors = "truepost") {
        add_header 'Access-Control-Allow-Origin' "$http_origin";
        add_header 'Access-Control-Allow-Credentials' 'true';
        add_header 'Access-Control-Allow-Methods' 'GET, POST, OPTIONS';
        add_header 'Access-Control-Allow-Headers' 'DNT,X-CustomHeader,Keep-Alive,User-Agent,X-Requested-With,If-Modified-Since,Cache-Control,Content-Type';
    }

}
```

</details>
