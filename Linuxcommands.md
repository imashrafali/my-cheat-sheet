 # Linux Command Line


| **Command** |  **Description**  |  
|  # arch  |  show architecture of machine(1)   [[man][1]]  |  
|  # cal 2007  |  show the timetable of 2007   [[man][2]]  |  
|  # cat /proc/cpuinfo  |  show information CPU info   [[man][3]]  |  
|  # cat /proc/interrupts  |  show interrupts   [[man][3]]  |  
|  # cat /proc/meminfo  |  verify memory use   [[man][3]]  |  
|  # cat /proc/swaps  |  show file(s) swap   [[man][3]]  |  
|  # cat /proc/version  |  show version of the kernel   [[man][3]]  |  
|  # cat /proc/net/dev  |  show network adpters and statistics   [[man][3]]  |  
|  # cat /proc/mounts  |  show mounted file system(s)   [[man][3]]  |  
|  # clock -w  |  save date changes on BIOS   [[man][4]]  |  
|  # date  |  show system date   [[man][5]]  |  
|  # date 041217002007.00  |  set date and time - MonthDayhoursMinutesYear.Seconds   [[man][5]]  |  
|  # dmidecode -q  |  show hardware system components - (SMBIOS / DMI)   [[man][6]]  |  
|  # hdparm -i /dev/hda  |  displays the characteristics of a hard-disk   [[man][7]]  |  
|  # hdparm -tT /dev/sda  |  perform test reading on a hard-disk   [[man][7]]  |  
|  # lspci -tv  |  display PCI devices   [[man][8]]  |  
|  # lsusb -tv  |  show USB devices   [[man][9]]  |  
|  # uname -m  |  show architecture of machine(2)   [[man][10]]  |  
|  # uname -r  |  show used kernel version   [[man][10]]  | 

 |  
| **Command** |  **Description**  |  
|  # init 0  |  shutdown system(2)   [[man][12]]  |  
|  # logout  |  leaving session   [[man][13]]  |  
|  # reboot  |  reboot(2)   [[man][14]]  |  
|  # shutdown -h now  |  shutdown system(1)   [[man][15]]  |  
|  # shutdown -h 16:30 &  |  planned shutdown of the system   [[man][15]]  |  
|  # shutdown -c  |  cancel a planned shutdown of the system   [[man][15]]  |  
|  # shutdown -r now  |  reboot(1)   [[man][15]]  |  
|  # telinit 0  |  shutdown system(3)   [[man][16]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # cd /home  |  enter to directory '/ home'   [[man][17]]  |  
|  # cd ..  |  go back one level   [[man][17]]  |  
|  # cd ../..  |  go back two levels   [[man][17]]  |  
|  # cd  |  go to home directory   [[man][17]]  |  
|  # cd ~user1  |  go to home directory   [[man][17]]  |  
|  # cd -  |  go to previous directory   [[man][17]]  |  
|  # cp file1 file2  |  copying a file   [[man][18]]  |  
|  # cp dir/* .  |  copy all files of a directory within the current work directory   [[man][18]]  |  
|  # cp -a /tmp/dir1 .  |  copy a directory within the current work directory   [[man][18]]  |  
|  # cp -a dir1 dir2  |  copy a directory   [[man][18]]  |  
|  # cp file file1  |  outputs the mime type of the file as text   [[man][19]]  |  
|  # iconv -l  |  lists known encodings   [[man][20]]  |  
|  # iconv -f fromEncoding -t toEncoding inputFile > outputFile  |  converting the coding of characters from one format to another   [[man][20]]  |  
|  # find . -maxdepth 1 -name *.jpg -print -exec convert  |  batch resize files in the current directory and send them to a thumbnails directory (requires convert from Imagemagick)   [[man][20]]  |  
|  # ln -s file1 lnk1  |  create a symbolic link to file or directory   [[man][21]]  |  
|  # ln file1 lnk1  |  create a physical link to file or directory   [[man][21]]  |  
|  # ls  |  view files of directory   [[man][22]]  |  
|  # ls -F  |  view files of directory   [[man][22]]  |  
|  # ls -l  |  show details of files and directory   [[man][22]]  |  
|  # ls -a  |  show hidden files   [[man][22]]  |  
|  # ls [*0-9]*  |  show files and directory containing numbers   [[man][22]]  |  
|  # lstree  |  show files and directories in a tree starting from root(2)   [[man][23]]  |  
|  # mkdir dir1  |  create a directory called 'dir1'   [[man][24]]  |  
|  # mkdir dir1 dir2  |  create two directories simultaneously   [[man][24]]  |  
|  # mkdir -p /tmp/dir1/dir2  |  create a directory tree   [[man][24]]  |  
|  # mv dir1 new_dir  |  rename / move a file or directory   [[man][25]]  |  
|  # pwd  |  show the path of work directory   [[man][26]]  |  
|  # rm -f file1  |  delete file called 'file1'   [[man][27]]  |  
|  # rm -rf dir1  |  remove a directory called 'dir1' and contents recursively   [[man][27]]  |  
|  # rm -rf dir1 dir2  |  remove two directories and their contents recursively   [[man][27]]  |  
|  # rmdir dir1  |  delete directory called 'dir1'   [[man][28]]  |  
|  # touch -t 0712250000 file1  |  modify timestamp of a file or directory - (YYMMDDhhmm)   [[man][29]]  |  
|  # tree  |  show files and directories in a tree starting from root(1)   [[man][30]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # find / -name file1  |  search file and directory into root filesystem from '/'   [[man][31]]  |  
|  # find / -user user1  |  search files and directories belonging to 'user1'   [[man][31]]  |  
|  # find /home/user1 -name *.bin  |  search files with '. bin' extension within directory '/ home/user1'   [[man][31]]  |  
|  # find /usr/bin -type f -atime +100  |  search binary files are not used in the last 100 days   [[man][31]]  |  
|  # find /usr/bin -type f -mtime -10  |  search files created or changed within 10 days   [[man][31]]  |  
|  # find / -name *.rpm -exec chmod 755 '{}' ;  |  search files with '.rpm' extension and modify permits   [[man][31]]  |  
|  # find / -xdev -name *.rpm  |  search files with '.rpm' extension ignoring removable partitions as cdrom, pen-drive, etc.…   [[man][31]]  |  
|  # locate *.ps  |  find files with the '.ps' extension - first run 'updatedb' command   [[man][32]]  |  
|  # whereis halt  |  show location of a binary file, source or man   [[man][33]]  |  
|  # which halt  |  show full path to a binary / executable   [[man][34]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # fuser -km /mnt/hda2  |  force umount when the device is busy   [[man][35]]  |  
|  # mount /dev/hda2 /mnt/hda2  |  mount disk called hda2 - verify existence of the directory '/ mnt/hda2'   [[man][36]]  |  
|  # mount /dev/fd0 /mnt/floppy  |  mount a floppy disk   [[man][36]]  |  
|  # mount /dev/cdrom /mnt/cdrom  |  mount a cdrom / dvdrom   [[man][36]]  |  
|  # mount /dev/hdc /mnt/cdrecorder  |  mount a cdrw / dvdrom   [[man][36]]  |  
|  # mount /dev/hdb /mnt/cdrecorder  |  mount a cdrw / dvdrom   [[man][36]]  |  
|  # mount -o loop file.iso /mnt/cdrom  |  mount a file or iso image   [[man][36]]  |  
|  # mount -t vfat /dev/hda5 /mnt/hda5  |  mount a Windows FAT32 file system   [[man][36]]  |  
|  # mount /dev/sda1 /mnt/usbdisk  |  mount a usb pen-drive or flash-drive   [[man][36]]  |  
|  # mount -t smbfs -o username=user,password=pass //WinClient/share /mnt/share  |  mount a windows network share   [[man][36]]  |  
|  # umount /dev/hda2  |  unmount disk called hda2 - exit from mount point '/ mnt/hda2' first   [[man][37]]  |  
|  # umount -n /mnt/hda2  |  run umount without writing the file /etc/mtab - useful when the file is read-only or the hard disk is full   [[man][37]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # df -h  |  show list of partitions mounted   [[man][38]]  |  
|  # dpkg-query -W -f='${Installed-Size;10}t${Package}n' | sort -k1,1n  |  show the used space by installed deb packages, sorting by size (debian, ubuntu and alike)   [[man][39]]  |  
|  # du -sh dir1  |  estimate space used by directory 'dir1'   [[man][40]]  |  
|  # du -sk * | sort -rn  |  show size of the files and directories sorted by size   [[man][40]]  |  
|  # ls -lSr |more  |  show size of the files and directories ordered by size   [[man][22]]  |  
|  # rpm -q -a --qf '%10{SIZE}t%{NAME}n' | sort -k1,1n  |  show space used by rpm packages installed sorted by size (fedora, redhat and like)   [[man][41]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # chage -E 2005-12-31 user1  |  set deadline for user password   [[man][42]]  |  
|  # groupadd [group]  |  create a new group   [[man][43]]  |  
|  # groupdel [group]  |  delete a group   [[man][44]]  |  
|  # groupmod -n moon sun  |  rename a group from moon to sun   [[man][45]]  |  
|  # grpck  |  check correct syntax and file format of '/etc/group' and groups existence   [[man][46]]  |  
|  # newgrp - [group]  |  log into a new group to change default group of newly created files   [[man][47]]  |  
|  # passwd  |  change password   [[man][48]]  |  
|  # passwd user1  |  change a user password (only by root)   [[man][48]]  |  
|  # pwck  |  check correct syntax and file format of '/etc/passwd' and users existence   [[man][49]]  |  
|  # useradd -c "User Linux" -g admin -d /home/user1 -s /bin/bash user1  |  create a new user "user1" belongs "admin" group   [[man][50]]  |  
|  # useradd user1  |  create a new user   [[man][50]]  |  
|  # userdel -r user1  |  delete a user ( '-r' eliminates home directory)   [[man][51]]  |  
|  # usermod -c "User FTP" -g system -d /ftp/user1 -s /bin/nologin user1  |  change user attributes   [[man][52]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # chgrp group1 file1  |  change group of files   [[man][53]]  |  
|  # chmod ugo+rwx directory1  |  set permissions reading (r), write (w) and (x) access to users owner (u) group (g) and others (o)   [[man][54]]  |  
|  # chmod go-rwx directory1  |  remove permits reading (r), write (w) and (x) access to users group (g) and others (or   [[man][54]]  |  
|  # chmod u+s /bin/file1  |  set SUID bit on a binary file - the user that running that file gets same privileges as owner   [[man][54]]  |  
|  # chmod u-s /bin/file1  |  disable SUID bit on a binary file   [[man][54]]  |  
|  # chmod g+s /home/public  |  set SGID bit on a directory - similar to SUID but for directory   [[man][54]]  |  
|  # chmod g-s /home/public  |  disable SGID bit on a directory   [[man][54]]  |  
|  # chmod o+t /home/public  |  set STIKY bit on a directory - allows files deletion only to legitimate owners   [[man][54]]  |  
|  # chmod o-t /home/public  |  disable STIKY bit on a directory   [[man][54]]  |  
|  # chown user1 file1  |  change owner of a file   [[man][55]]  |  
|  # chown -R user1 directory1  |  change user owner of a directory and all the files and directories contained inside   [[man][55]]  |  
|  # chown user1:group1 file1  |  change user and group ownership of a file   [[man][55]]  |  
|  # find / -perm -u+s  |  view all files on the system with SUID configured   [[man][31]]  |  
|  # ls -lh  |  show permits on files   [[man][22]]  |  
|  # ls /tmp | pr -T5 -W$COLUMNS  |  divide terminal into 5 columns   [[man][22]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # chattr +a file1  |  allows write opening of a file only append mode   [[man][56]]  |  
|  # chattr +c file1  |  allows that a file is compressed / decompressed automatically by the kernel   [[man][56]]  |  
|  # chattr +d file1  |  makes sure that the program ignores Dump the files during backup   [[man][56]]  |  
|  # chattr +i file1  |  makes it an immutable file, which can not be removed, altered, renamed or linked   [[man][56]]  |  
|  # chattr +s file1  |  allows a file to be deleted safely   [[man][56]]  |  
|  # chattr +S file1  |  makes sure that if a file is modified changes are written in synchronous mode as with sync   [[man][56]]  |  
|  # chattr +u file1  |  allows you to recover the contents of a file even if it is canceled   [[man][56]]  |  
|  # lsattr  |  show specials attributes   [[man][57]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # bunzip2 file1.bz2  |  decompress a file called 'file1.bz2'   [[man][58]]  |  
|  # bzip2 file1  |  compress a file called 'file1'   [[man][59]]  |  
|  # gunzip file1.gz  |  decompress a file called 'file1.gz'   [[man][60]]  |  
|  # gzip file1  |  compress a file called 'file1'   [[man][61]]  |  
|  # gzip -9 file1  |  compress with maximum compression   [[man][61]]  |  
|  # rar a file1.rar test_file  |  create an archive rar called 'file1.rar'   [[man][62]]  |  
|  # rar a file1.rar file1 file2 dir1  |  compress 'file1', 'file2' and 'dir1' simultaneously   [[man][62]]  |  
|  # rar x file1.rar  |  decompress rar archive   [[man][62]]  |  
|  # tar -cvf archive.tar file1  |  create a uncompressed tarball   [[man][63]]  |  
|  # tar -cvf archive.tar file1 file2 dir1  |  create an archive containing 'file1', 'file2' and 'dir1'   [[man][63]]  |  
|  # tar -tf archive.tar  |  show contents of an archive   [[man][63]]  |  
|  # tar -xvf archive.tar  |  extract a tarball   [[man][63]]  |  
|  # tar -xvf archive.tar -C /tmp  |  extract a tarball into / tmp   [[man][63]]  |  
|  # tar -cvfj archive.tar.bz2 dir1  |  create a tarball compressed into bzip2   [[man][63]]  |  
|  # tar -xvfj archive.tar.bz2  |  decompress a compressed tar archive in bzip2   [[man][63]]  |  
|  # tar -cvfz archive.tar.gz dir1  |  create a tarball compressed into gzip   [[man][63]]  |  
|  # tar -xvfz archive.tar.gz  |  decompress a compressed tar archive in gzip   [[man][63]]  |  
|  # unrar x file1.rar  |  decompress rar archive   [[man][64]]  |  
|  # unzip file1.zip  |  decompress a zip archive   [[man][65]]  |  
|  # zip file1.zip file1  |  create an archive compressed in zip   [[man][66]]  |  
|  # zip -r file1.zip file1 file2 dir1  |  compress in zip several files and directories simultaneously   [[man][66]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # rpm -ivh [package.rpm]  |  install a rpm package   [[man][41]]  |  
|  # rpm -ivh --nodeeps [package.rpm]  |  install a rpm package ignoring dependencies requests   [[man][41]]  |  
|  # rpm -U [package.rpm]  |  upgrade a rpm package without changing configuration files   [[man][41]]  |  
|  # rpm -F [package.rpm]  |  upgrade a rpm package only if it is already installed   [[man][41]]  |  
|  # rpm -e [package]  |  remove a rpm package   [[man][41]]  |  
|  # rpm -qa  |  show all rpm packages installed on the system   [[man][41]]  |  
|  # rpm -qa | grep httpd  |  show all rpm packages with the name "httpd"   [[man][41]]  |  
|  # rpm -qi [package]  |  obtain information on a specific package installed   [[man][41]]  |  
|  # rpm -qg "System Environment/Daemons"  |  show rpm packages of a group software   [[man][41]]  |  
|  # rpm -ql [package]  |  show list of files provided by a rpm package installed   [[man][41]]  |  
|  # rpm -qc [package]  |  show list of configuration files provided by a rpm package installed   [[man][41]]  |  
|  # rpm -q [package] --whatrequires  |  show list of dependencies required for a rpm packet   [[man][41]]  |  
|  # rpm -q [package] --whatprovides  |  show capability provided by a rpm package   [[man][41]]  |  
|  # rpm -q [package] --scripts  |  show scripts started during installation / removal   [[man][41]]  |  
|  # rpm -q [package] --changelog  |  show history of revisions of a rpm package   [[man][41]]  |  
|  # rpm -qf /etc/httpd/conf/httpd.conf  |  verify which rpm package belongs to a given file   [[man][41]]  |  
|  # rpm -qp [package.rpm] -l  |  show list of files provided by a rpm package not yet installed   [[man][41]]  |  
|  # rpm --import /media/cdrom/RPM-GPG-KEY  |  import public-key digital signature   [[man][41]]  |  
|  # rpm --checksig [package.rpm]  |  verify the integrity of a rpm package   [[man][41]]  |  
|  # rpm -qa gpg-pubkey  |  verify integrity of all rpm packages installed   [[man][41]]  |  
|  # rpm -V [package]  |  check file size, permissions, type, owner, group, MD5 checksum and last modification   [[man][41]]  |  
|  # rpm -Va  |  check all rpm packages installed on the system - use with caution   [[man][41]]  |  
|  # rpm -Vp [package.rpm]  |  verify a rpm package not yet installed   [[man][41]]  |  
|  # rpm -ivh /usr/src/redhat/RPMS/`arch`/[package.rpm]  |  install a package built from a rpm source   [[man][41]]  |  
|  # rpm2cpio [package.rpm] | cpio --extract --make-directories *bin*  |  extract executable file from a rpm package   [[man][67]]  |  
|  # rpmbuild --rebuild [package.src.rpm]  |  build a rpm package from a rpm source   [[man][68]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # yum -y install [package]  |  download and install a rpm package   [[man][69]]  |  
|  # yum localinstall [package.rpm]  |  That will install an RPM, and try to resolve all the dependencies for you using your repositories.   [[man][69]]  |  
|  # yum -y update  |  update all rpm packages installed on the system   [[man][69]]  |  
|  # yum update [package]  |  upgrade a rpm package   [[man][69]]  |  
|  # yum remove [package]  |  remove a rpm package   [[man][69]]  |  
|  # yum list  |  list all packages installed on the system   [[man][69]]  |  
|  # yum search [package]  |  find a package on rpm repository   [[man][69]]  |  
|  # yum clean [package]  |  clean up rpm cache erasing downloaded packages   [[man][69]]  |  
|  # yum clean headers  |  remove all files headers that the system uses to resolve dependency   [[man][69]]  |  
|  # yum clean all  |  remove from the cache packages and headers files   [[man][69]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # dpkg -i [package.deb]  |  install / upgrade a deb package   [[man][39]]  |  
|  # dpkg -r [package]  |  remove a deb package from the system   [[man][39]]  |  
|  # dpkg -l  |  show all deb packages installed on the system   [[man][39]]  |  
|  # dpkg -l | grep httpd  |  show all deb packages with the name "httpd"   [[man][39]]  |  
|  # dpkg -s [package]  |  obtain information on a specific package installed on system   [[man][39]]  |  
|  # dpkg -L [package]  |  show list of files provided by a package installed on system   [[man][39]]  |  
|  # dpkg --contents [package.deb]  |  show list of files provided by a package not yet installed   [[man][39]]  |  
|  # dpkg -S /bin/ping  |  verify which package belongs to a given file   [[man][39]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # apt-cache search [package]  |  returns list of packages which corresponds string "searched-packages"   [[man][70]]  |  
|  # apt-cdrom install [package]  |  install / upgrade a deb package from cdrom   [[man][71]]  |  
|  # apt-get install [package]  |  install / upgrade a deb package   [[man][72]]  |  
|  # apt-get update  |  update the package list   [[man][72]]  |  
|  # apt-get upgrade  |  upgrade all of the installed packages   [[man][72]]  |  
|  # apt-get remove [package]  |  remove a deb package from system   [[man][72]]  |  
|  # apt-get check  |  verify correct resolution of dependencies   [[man][72]]  |  
|  # apt-get clean  |  clean up cache from packages downloaded   [[man][72]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # pacman -S name  |  Install package 'name' with dependencies   [[man][73]]  |  
|  # pacman -R name  |  Delete package 'name' and all files of it   [[man][73]]  | 

 |  
|  **«** [**TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # cat file1  |  view the contents of a file starting from the first row   [[man][3]]  |  
|  # head -2 file1  |  view first two lines of a file   [[man][74]]  |  
|  # less file1  |  similar to 'more' command but which allows backward movement in the file as well as forward movement   [[man][75]]  |  
|  # more file1  |  view content of a file along   [[man][76]]  |  
|  # tac file1  |  view the contents of a file starting from the last line   [[man][77]]  |  
|  # tail -2 file1  |  view last two lines of a file   [[man][78]]  |  
|  # tail -f /var/log/messages  |  view in real time what is added to a file   [[man][78]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # cat example.txt | awk 'NR%2==1'  |  remove all even lines from example.txt   [[man][79]]  |  
|  # echo a b c | awk '{print $1}'  |  view the first column of a line   [[man][79]]  |  
|  # echo a b c | awk '{print $1,$3}'  |  view the first and third column of a line   [[man][79]]  |  
|  # cat -n file1  |  number row of a file   [[man][3]]  |  
|  # comm -1 file1 file2  |  compare contents of two files by deleting only unique lines from 'file1'   [[man][80]]  |  
|  # comm -2 file1 file2  |  compare contents of two files by deleting only unique lines from 'file2'   [[man][80]]  |  
|  # comm -3 file1 file2  |  compare contents of two files by deleting only the lines that appear on both files   [[man][80]]  |  
|  # diff file1 file2  |  find differences between two files   [[man][81]]  |  
|  # grep Aug /var/log/messages  |  look up words "Aug" on file '/var/log/messages'   [[man][82]]  |  
|  # grep ^Aug /var/log/messages  |  look up words that begin with "Aug" on file '/var/log/messages'   [[man][82]]  |  
|  # grep [0-9] /var/log/messages  |  select from file '/var/log/messages' all lines that contain numbers   [[man][82]]  |  
|  # grep Aug -R /var/log/*  |  search string "Aug" at directory '/var/log' and below   [[man][82]]  |  
|  # paste file1 file2  |  merging contents of two files for columns   [[man][83]]  |  
|  # paste -d '+' file1 file2  |  merging contents of two files for columns with '+' delimiter on the center   [[man][83]]  |  
|  # sdiff file1 file2  |  find differences between two files and merge interactively alike "diff"   [[man][84]]  |  
|  # sed 's/string1/string2/g' example.txt  |  replace "string1" with "string2" in example.txt   [[man][85]]  |  
|  # sed '/^$/d' example.txt  |  remove all blank lines from example.txt   [[man][85]]  |  
|  # sed '/ *#/d; /^$/d' example.txt  |  remove comments and blank lines from example.txt   [[man][85]]  |  
|  # sed -e '1d' exampe.txt  |  eliminates the first line from file example.txt   [[man][85]]  |  
|  # sed -n '/string1/p'  |  view only lines that contain the word "string1"   [[man][85]]  |  
|  # sed -e 's/ *$//' example.txt  |  remove empty characters at the end of each row   [[man][85]]  |  
|  # sed -e 's/string1//g' example.txt  |  remove only the word "string1" from text and leave intact all   [[man][85]]  |  
|  # sed -n '1,5p' example.txt  |  print from 1th to 5th row of example.txt   [[man][85]]  |  
|  # sed -n '5p;5q' example.txt  |  print row number 5 of example.txt   [[man][85]]  |  
|  # sed -e 's/00*/0/g' example.txt  |  replace more zeros with a single zero   [[man][85]]  |  
|  # sort file1 file2  |  sort contents of two files   [[man][86]]  |  
|  # sort file1 file2 | uniq  |  sort contents of two files omitting lines repeated   [[man][86]]  |  
|  # sort file1 file2 | uniq -u  |  sort contents of two files by viewing only unique line   [[man][86]]  |  
|  # sort file1 file2 | uniq -d  |  sort contents of two files by viewing only duplicate line   [[man][86]]  |  
|  # echo 'word' | tr '[:lower:]' '[:upper:]'  |  convert from lower case in upper case   [[man][87]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # dos2unix filedos.txt fileunix.txt  |  convert a text file format from MSDOS to UNIX   [[man][88]]  |  
|  # recode ..HTML page.html  |  convert a text file to html   [[man][89]]  |  
|  # recode -l | more  |  show all available formats conversion   [[man][89]]  |  
|  # unix2dos fileunix.txt filedos.txt  |  convert a text file format from UNIX to MSDOS   [[man][90]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # badblocks -v /dev/hda1  |  check bad blocks on disk hda1   [[man][91]]  |  
|  # dosfsck /dev/hda1  |  repair / check integrity of dos filesystems on disk hda1   [[man][92]]  |  
|  # e2fsck /dev/hda1  |  repair / check integrity of ext2 filesystem on disk hda1   [[man][93]]  |  
|  # e2fsck -j /dev/hda1  |  repair / check integrity of ext3 filesystem on disk hda1   [[man][93]]  |  
|  # fsck /dev/hda1  |  repair / check integrity of linux filesystem on disk hda1   [[man][94]]  |  
|  # fsck.ext2 /dev/hda1  |  repair / check integrity of ext2 filesystem on disk hda1   [[man][94]]  |  
|  # fsck.ext3 /dev/hda1  |  repair / check integrity of ext3 filesystem on disk hda1   [[man][94]]  |  
|  # fsck.vfat /dev/hda1  |  repair / check integrity of fat filesystem on disk hda1   [[man][94]]  |  
|  # fsck.msdos /dev/hda1  |  repair / check integrity of dos filesystem on disk hda1   [[man][94]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # fdformat -n /dev/fd0  |  format a floppy disk   [[man][95]]  |  
|  # mke2fs /dev/hda1  |  create a filesystem type linux ext2 on hda1 partition   [[man][96]]  |  
|  # mke2fs -j /dev/hda1  |  create a filesystem type linux ext3 (journal) on hda1 partition   [[man][96]]  |  
|  # mkfs /dev/hda1  |  create a filesystem type linux on hda1 partition   [[man][97]]  |  
|  # mkfs -t vfat 32 -F /dev/hda1  |  create a FAT32 filesystem   [[man][97]]  |  
|  # mkswap /dev/hda3  |  create a swap filesystem   [[man][98]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # mkswap /dev/hda3  |  create a swap filesystem   [[man][98]]  |  
|  # swapon /dev/hda3  |  activating a new swap partition   [[man][99]]  |  
|  # swapon /dev/hda2 /dev/hdb3  |  activate two swap partitions   [[man][99]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # find /var/log -name '*.log' | tar cv --files-from=- | bzip2 > log.tar.bz2  |  find all files with '.log' extention and make an bzip archive   [[man][59]]  |  
|  # find /home/user1 -name '*.txt' | xargs cp -av --target-directory=/home/backup/ --parents  |  find and copy all files with '.txt' extention from a directory to another   [[man][18]]  |  
|  # dd bs=1M if=/dev/hda | gzip | ssh user@ip_addr 'dd of=hda.gz'  |  make a backup of a local hard disk on remote host via ssh   [[man][100]]  |  
|  # dd if=/dev/sda of=/tmp/file1  |  backup content of the harddrive to a file   [[man][100]]  |  
|  # dd if=/dev/hda of=/dev/fd0 bs=512 count=1  |  make a copy of MBR (Master Boot Record) to floppy   [[man][100]]  |  
|  # dd if=/dev/fd0 of=/dev/hda bs=512 count=1  |  restore MBR from backup copy saved to floppy   [[man][100]]  |  
|  # dump -0aj -f /tmp/home0.bak /home  |  make a full backup of directory '/home'   [[man][101]]  |  
|  # dump -1aj -f /tmp/home0.bak /home  |  make a incremental backup of directory '/home'   [[man][101]]  |  
|  # restore -if /tmp/home0.bak  |  restoring a backup interactively   [[man][102]]  |  
|  # rsync -rogpav --delete /home /tmp  |  synchronization between directories   [[man][103]]  |  
|  # rsync -rogpav -e ssh --delete /home ip_address:/tmp  |  rsync via SSH tunnel   [[man][103]]  |  
|  # rsync -az -e ssh --delete ip_addr:/home/public /home/local  |  synchronize a local directory with a remote directory via ssh and compression   [[man][103]]  |  
|  # rsync -az -e ssh --delete /home/local ip_addr:/home/public  |  synchronize a remote directory with a local directory via ssh and compression   [[man][103]]  |  
|  # tar -Puf backup.tar /home/user  |  make a incremental backup of directory '/home/user'   [[man][63]]  |  
|  # ( cd /tmp/local/ && tar c . ) | ssh -C user@ip_addr 'cd /home/share/ && tar x -p'  |  copy content of a directory on remote directory via ssh   [[man][63]]  |  
|  # ( tar c /home ) | ssh -C user@ip_addr 'cd /home/backup-home && tar x -p'  |  copy a local directory on remote directory via ssh   [[man][63]]  |  
|  # tar cf - . | (cd /tmp/backup ; tar xf - )  |  local copy preserving permits and links from a directory to another   [[man][63]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # cd-paranoia -B  |  rip audio tracks from a CD to wav files   [[man][104]]  |  
|  # cd-paranoia --  |  rip first three audio tracks from a CD to wav files   [[man][104]]  |  
|  # cdrecord -v gracetime=2 dev=/dev/cdrom -eject blank=fast -force  |  clean a rewritable cdrom   [[man][105]]  |  
|  # cdrecord -v dev=/dev/cdrom cd.iso  |  burn an ISO image   [[man][105]]  |  
|  # gzip -dc cd_iso.gz | cdrecord dev=/dev/cdrom -  |  burn a compressed ISO image   [[man][105]]  |  
|  # cdrecord --scanbus  |  scan bus to identify the channel scsi   [[man][105]]  |  
|  # dd if=/dev/hdc | md5sum  |  perform an md5sum on a device, like a CD   [[man][106]]  |  
|  # mkisofs /dev/cdrom > cd.iso  |  create an iso image of cdrom on disk   [[man][107]]  |  
|  # mkisofs /dev/cdrom | gzip > cd_iso.gz  |  create a compressed iso image of cdrom on disk   [[man][107]]  |  
|  # mkisofs -J -allow-leading-dots -R -V  |  create an iso image of a directory   [[man][107]]  |  
|  # mount -o loop cd.iso /mnt/iso  |  mount an ISO image   [[man][36]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # dhclient eth0  |  active interface 'eth0' in dhcp mode   [[man][108]]  |  
|  # ethtool eth0  |  show network statistics of eth0   [[man][109]]  |  
|  # host www.example.com  |  lookup hostname to resolve name to ip address and viceversa   [[man][110]]  |  
|  # hostname  |  show hostname of system   [[man][111]]  |  
|  # ifconfig eth0  |  show configuration of an ethernet network card   [[man][112]]  |  
|  # ifconfig eth0 192.168.1.1 netmask 255.255.255.0  |  configure IP Address   [[man][112]]  |  
|  # ifconfig eth0 promisc  |  configure 'eth0' in promiscuous mode to gather packets (sniffing)   [[man][112]]  |  
|  # ifdown eth0  |  disable an interface 'eth0'   [[man][113]]  |  
|  # ifup eth0  |  activate an interface 'eth0'   [[man][114]]  |  
|  # ip link show  |  show link status of all network interfaces   [[man][115]]  |  
|  # iwconfig eth1  |  show wireless networks   [[man][116]]  |  
|  # iwlist scan  |  wifi scanning to display the wireless connections available   [[man][117]]  |  
|  # mii-tool eth0  |  show link status of 'eth0'   [[man][118]]  |  
|  # netstat -tup  |  show all active network connections and their PID   [[man][119]]  |  
|  # netstat -tupl  |  show all network services listening on the system and their PID   [[man][119]]  |  
|  # netstat -rn  |  show routing table alike "route -n"   [[man][119]]  |  
|  # nslookup www.example.com  |  lookup hostname to resolve name to ip address and viceversa   [[man][120]]  |  
|  # route -n  |  show routing table   [[man][121]]  |  
|  # route add -net 0/0 gw IP_Gateway  |  configure default gateway   [[man][121]]  |  
|  # route add -net 192.168.0.0 netmask 255.255.0.0 gw 192.168.1.1  |  configure static route to reach network '192.168.0.0/16'   [[man][121]]  |  
|  # route del 0/0 gw IP_gateway  |  remove static route   [[man][121]]  |  
|  # echo "1" > /proc/sys/net/ipv4/ip_forward  |  activate ip routing   [[man][121]]  |  
|  # tcpdump tcp port 80  |  show all HTTP traffic   [[man][122]]  |  
|  # whois www.example.com  |  lookup on Whois database   [[man][123]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # mount -t smbfs -o username=user,password=pass //WinClient/share /mnt/share  |  mount a windows network share   [[man][36]]  |  
|  # nbtscan ip_addr  |  netbios name resolution   [[man][124]]  |  
|  # nmblookup -A ip_addr  |  netbios name resolution   [[man][125]]  |  
|  # smbclient -L ip_addr/hostname  |  show remote shares of a windows host   [[man][126]]  |  
|  # smbget -Rr smb://ip_addr/share  |  like wget can download files from a host windows via smb   [[man][127]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # iptables -t filter -L  |  show all chains of filtering table   [[man][128]]  |  
|  # iptables -t nat -L  |  show all chains of nat table   [[man][128]]  |  
|  # iptables -t filter -F  |  clear all rules from filtering table   [[man][128]]  |  
|  # iptables -t nat -F  |  clear all rules from table nat   [[man][128]]  |  
|  # iptables -t filter -X  |  delete any chains created by user   [[man][128]]  |  
|  # iptables -t filter -A INPUT -p tcp --dport telnet -j ACCEPT  |  allow telnet connections to input   [[man][128]]  |  
|  # iptables -t filter -A OUTPUT -p tcp --dport http -j DROP  |  block HTTP connections to output   [[man][128]]  |  
|  # iptables -t filter -A FORWARD -p tcp --dport pop3 -j ACCEPT  |  allow POP3 connections to forward chain   [[man][128]]  |  
|  # iptables -t filter -A INPUT -j LOG --log-prefix  |  Logging on input chain   [[man][128]]  |  
|  # iptables -t nat -A POSTROUTING -o eth0 -j MASQUERADE  |  configure a PAT (Port Address Traslation) on eth0 masking outbound packets   [[man][128]]  |  
|  # iptables -t nat -A PREROUTING -d 192.168.0.1 -p tcp -m tcp --dport 22 -j DNAT --to-destination 10.0.0.2:22  |  redirect packets addressed to a host to another host   [[man][128]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # free -m  |  displays status of RAM in megabytes   [[man][129]]  |  
|  # kill -9 process_id  |  force closure of the process and finish it   [[man][130]]  |  
|  # kill -1 process_id  |  force a process to reload configuration   [[man][130]]  |  
|  # last reboot  |  show history reboot   [[man][131]]  |  
|  # lsmod  |  display kernel loaded   [[man][132]]  |  
|  # lsof -p process_id  |  display a list of files opened by processes   [[man][133]]  |  
|  # lsof /home/user1  |  displays a list of open files in a given path system   [[man][133]]  |  
|  # ps -eafw  |  displays linux tasks   [[man][134]]  |  
|  # ps -e -o pid,args --forest  |  displays linux tasks in a hierarchical mode   [[man][134]]  |  
|  # pstree  |  Shows a tree system processes   [[man][135]]  |  
|  # smartctl -A /dev/hda  |  monitoring reliability of a hard-disk through SMART   [[man][136]]  |  
|  # smartctl -i /dev/hda  |  check if SMART is active on a hard-disk   [[man][136]]  |  
|  # strace -c ls >/dev/null  |  display system calls made and received by a process   [[man][137]]  |  
|  # strace -f -e open ls >/dev/null  |  display library calls   [[man][137]]  |  
|  # tail /var/log/dmesg  |  show events inherent to the process of booting kernel   [[man][78]]  |  
|  # tail /var/log/messages  |  show system events   [[man][78]]  |  
|  # top  |  display linux tasks using most cpu   [[man][138]]  |  
|  # watch -n1 'cat /proc/interrupts'  |  display interrupts in real-time   [[man][139]]  | 

 |  
|  **«** **[TOP**][11] **«** |  
|  |  
| 

|   |  
| **Command** |  **Description**  |  
|  # alias hh='history'  |  set an alias for a command - hh = history   [[man][140]]  |  
|  # apropos ...keyword  |  display a list of commands that pertain to keywords of a program , useful when you know what your program does, but you don't know the name of the command   [[man][141]]  |  
|  # chsh  |  change shell command   [[man][142]]  |  
|  # chsh --list-shells  |  nice command to know if you have to remote into another box   [[man][142]]  |  
|  # gpg -c file1  |  encrypt a file with GNU Privacy Guard   [[man][143]]  |  
|  # gpg file1.gpg  |  decrypt a file with GNU Privacy Guard   [[man][143]]  |  
|  # ldd /usr/bin/ssh  |  show shared libraries required by ssh program   [[man][144]]  |  
|  # man ping  |  display the on-line manual pages for example on ping command - use '-k' option to find any related commands   [[man][145]]  |  
|  # mkbootdisk --device /dev/fd0 `uname -r`  |  create a boot floppy   [[man][146]]  |  
|  # wget -r www.example.com  |  download an entire web site   [[man][147]]  |  
|  # wget -c www.example.com/file.iso  |  download a file with the ability to stop the download and resume later   [[man][147]]  |  
|  # echo 'wget -c www.example.com/files.iso' | at 09:00  |  start a download at any given time   [[man][147]]  |  
|  # whatis ...keyword  |  displays description of what a program does   [[man][148]]  |  
|  # who -a  |  show who is logged on, and print: time of last system boot, dead processes, system login processes, active processes spawned by init, current runlevel, last system clock change   [[man][149]]  | 

© 2021 GitHub, Inc.
Terms
Privacy
Security
Status
Help
Contact GitHub
Pricing
API
Training
Blog
About
