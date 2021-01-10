# SYSTEM
## linux-system

```
$ uname -a Displays Linux system information

$ uname -r Displays kernel release information

$ uptime Shows how long system running + load

$ hostname Shows system host name

$ hostname -i  Displays the IP address of the host

$ last reboot Shows system reboot history

$ date Shows the current date and time

$ cal Shows this month calendar

$ whoami Shows who you are logged in as
```

# HARDWARE
## linux-hardware

```
$ dmesg Detected hardware and boot messages

$ cat /proc/meminfo Hardware memory information

$ cat /proc/cpuinfo CPU model information

$ cat /proc/interrupts Lists the number of interrupts per CPU per I/O device

$ sudo lshw Displays information on hardware configuration of the system

$ lsblk Displays block device related information in Linux (sudo yum install util-linux-ng)

$ free -m Displays used and free memory (-m for MB)

$ lsusb -tv Shows USB devices

$ sudo dmidecode Shows hardware info from the BIOS

$ sudo hdparm -i /dev/sda # Shows info about disk sda

$ sudo hdparm -tT /dev/sda # Do a read speed test on disk sda

$ sudo badblocks -s /dev/sda # Test for unreadable blocks on disk sda
```

# STATISTICS
## linux-statistics

```
$ top Displays the top CPU processes (Ctrl+C to exit)

$ vmstat 2 Displays virtual memory statistics

$ sudo tcpdump -i eth0 Captures all packets flows on interface eth0

$ sudo tcpdump -i eth0 'port 80' Monitors all traffic on port 80 ( HTTP )

$ lsof Lists all open files belonging to all active processes.

$ lsof -u myuser Lists files opened by specific user

$ watch df -h Shows changeable data continuously

```
# USERS
## linux-users

```
$ id Shows the active user id with login and group

$ last Shows last logins on the system

$ who Shows who is logged on the system

$ groupadd admin Adds group "admin" 

$ useradd -c "Sam Tomshi" -g admin -m sam Creates user "sam" and adds to group "admin"

$ userdel sam Deletes user sam

$ adduser sam Adds user "sam"

$ usermod Modifies user information
```

# FILE COMMANDS
## linux-file

```
$ cd .. To go up one level of the directory tree

$ cd Goes to $HOME directory

$ cd /test Changes to /test directory

$ ls gives the contents of a folder.

$ ls -a gives all the contents of a folder.

$ mkdir FolderName creates the folder FolderName.

$ cd Directory makes the Directory current directory

$ pwd prints the working directory

$ cp ~/Desktop/Berk/backups/science.txt . copy science.txt to the current directory

$ mv backups/science.txt /Desktop/Emi moves science.txt to folder Emi

$ rm temp.txt removes the temp.txt file

$ clear clear screen

$ cat science.txt Display contents of a file on the screen

$ less science.txt Displays on a different page ( type q to close the page)

$ less science.txt and then /name finds the occurences of name

$ head science.txt displays the first ten lines of the file

$ tail science.txt displays the last ten lines of the file

$ tail -20 science.txt displays the last 20 lines of the file

$ grep 'searchedkeyword' science.txt searches and finds the keyword in the file.(case sensitive)

$ grep -i SeaRchEdKeyWoRd science.txt case insensitive search

$ grep -i 'SeaRched Sentence is this one' science.txt case insensitive search

instead of i we can use;
-n precede each matching line with the line number
-v display those lines that do not match
-c print only the total count of matching lines

$ find -name "*.txt" -print  finds the text files in the current directory

$ diff a.txt b.txt gives the different lines

$ wc -w science.txt gives the word count

$ wc -l science.txt gives the line count

$ cat > list1
   pear
   banana
   ...
   ctrl+d

creates a list and we can print this list by using:

$ cat list1 command line.

$ cat biglist | grep p | sort gives sorted list elements which include p

$ sort < biglist > sortedlist sorts the biglist and writes it to the sortedlist

$ ls list* outputs the filenames starting with 'list'

$ ls *list outputs the filenames ending with 'list'

$ ls ?un outputs the filenames ending with 'un' but just one letter. (e.g. sun, gun, bun)

$ man ____ gives information about the command in the underlined section.

$ whatis ____ gives information about the command in the underlined section.

$ ls -l gives detailed information about the gfiles in the directory

u:user
g:group
o:other people
rwx: read write execute
rw: read write
r: read
x: execute

$ chmod u+x  TheFile adds writing permission to the user(owner) of TheFile

$ chmod go-rwx biglist to remove read write and execute permissions on the file biglist for the group and others

$ chmod 754 TheFile 7, 5, 4 represents the individual permissions for user, group, other (7:rwx, 5:rx, 4:r)

4 – stands for “read”
2 – stands for “write”
1 – stands for “execute”
0 – no permissions

$ du -s * The du command outputs the number of kilobyes used by each subdirectory.

$ df . The df command reports on the space left on the file system.

$ gzip science.txt Compresses into a gzip file

$ gunzip science.txt.gz De-compresses into the original file

$ tar cvf New.tar addthisfileintotar  Create a tar file called New and add this file.

$ tar xvf New.tar Extracts the tar file

$ zcat science.txt.gz reads zipped files without unzipping

$ file * Classifies the files in the current directory ( folder, text, gzip, etc.)

$ name=Berk
$ echo Hello $name  Prints 'Hello Berk'

$ sha1sum FileName | grep e509760917361307015  Compares the checksum of a downloaded file and the calculated one.

$ gpg -c file Encrypts file

$ gpg file.gpg Decrypts file

```
# PROCESS RELATED
## linux-process

```
$ ps Displays your currently active processes

$ ps aux | grep 'telnet' Finds all process id related to telnet process

$ pmap Memory map of process

$ top Display all running processes

$ kill pid Kill process with mentioned pid id

$ killall proc Kill all processes named proc

$ sleep 10 & Sleeps at the background

$ kill 'JobNumber '  Terminates the job

$ jobs Display the jobs 

$ pkill processname Send signal to a process with its name

$ bg Resumes suspended jobs without bringing them to foreground

$ fg Brings the most recent job to foreground

$ fg n Brings job n to the foreground

```
# FILE PERMISSION RELATED
## linux-permission

```
$ chmod 777 /data/test.c Sets rwx permission for owner , rwx permission for group, rwx permission for world

$ chmod 755 /data/test.c Sets rwx permission for owner,rx for group and world

$ chown owner-user file Changes the owner of the file

$ chown owner-user:owner-group file-name Changes the owner and group owner of the file

$ chown owner-user:owner-group directory Changes the owner and group owner of the directory

```
# NETWORK
## linux-network

```
$ ifconfig -a Display all network ports and ip address

$ ifconfig eth0 Display specific ethernet port ip address and details

$ ip addr show Display all network interfaces and ip address(available in iproute2 package,powerful than ifconfig)

$ ip address add 192.168.0.1 dev eth0 Set ip address

$ ethtool eth0 Linux tool to show ethernet status

$ mii-tool eth0 Linux tool to show ethernet status 

$ ping host Sends echo request to test connection

$ whois domain Get who is information for domain

$ dig domain Get DNS information for domain

$ dig -x host Reverse lookup host

$ host google.com Lookup DNS ip address for the name

$ hostname -i Lookup local ip address 

$ wget file  Download file

$ netstat -tupl Listing all active listening ports(tcp,udp,pid)

$ ssh user@host Connects to host as user

$ ssh -p port user@host Connects to host using specific port

$ telnet host Connects to the system using telnet port

```
# COMPRESSION / ARCHIVES
## linux-compression

```
$ tar cf home.tar home Creates tar named home.tar containing home/

$ tar xf file.tar Extracts the files from file.tar

$ tar czf file.tar.gz files Creates a tar with gzip compression

$ gzip file Compresses the file and renames it to file.gz

```
# FILE TRANSFER
## linux-file-transfer

```
$ scp file.txt server2:/tmp  Secure copies file.txt to remote host /tmp folder

$ scp nixsavy@server2:/www/*.html /www/tmp  Copies *.html files from remote host to current system /www/tmp folder

$ scp -r nixsavy@server2:/www /www/tmp Copies all files and folders recursively from remote server to the current system /www/tmp folder

$ rsync -a /home/apps /backup/ Synchronizes source to destination

$ rsync -avz /home/apps linoxide@192.168.10.1:/backup Synchronizes files/directories between the local and remote system with compression enabled
```
