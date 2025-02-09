## 1. File and Directory Management
```javascript
1. pwd
Prints the current working directory

2. ls	
Lists files and directories	

3. ls -a
Lists of all files and directory including they are hidden

4. ls -l 
(detailed list)

5. cd /home/user/Documents
Changes the directory

6. cd ..
move to previous/parent directory

7. mkdir new_folder
Creates a new directory	

8. rmdir old_folder
Removes an empty directory	

9. rm
Removes files or directories

10. rm -r my_folder 
removes non-empty dir

11. touch myfile.txt file1.txt file2.txt
Creates an empty file

12. cp file1.txt file2.txt
Copies files or directories	

13. mv oldname.txt newname.txt
Moves or renames files or directories	

14. find /home -name "*.txt"
Searches for files	
```


## 2. File Operations
```javascript
1. cat file.txt
Displays file content	

2. tac file.txt
Displays file content in reverse	

3. less file.txt
Views file content page by page	

4. more file.txt
Similar to less, but less interactive	

5. head -10 file.txt
Displays first N lines of a file	

6. tail -10 file.txt
Displays last N lines of a file	

7. diff file1.txt file2.txt
Compares two files line by line	

8. cmp file1.txt file2.txt
Compares two files byte by byte
```




## 3. File Permissions and Ownership
```javascript
1. ls -l file.txt
Displays file permissions

2. chmod 755 script.sh
Changes file permissions	

3. chown user <file.txt></file.txt>
Changes file owner	

4. chgrp developers file.txt
Changes group ownership	
```



## 4. Compression and Archiving
```javascript
1. tar -cvf archive.tar file.txt
Creates archive files	

2. tar -xvf archive.tar
extracts archive files

3. zip archive.zip file.txt
Compresses files into a .zip

4. unzip archive.zip
Extracts .zip files	

5. gzip file.txt
Compresses files with gzip	

6. gunzip file.txt.gz
Decompresses .gz files	
```



## 5. Disk and Storage Management
```javascript
1. df -h
Displays disk space usage	

2. du -sh /home/user
Shows disk usage of files and directories

3. lsblk 
Lists block devices	
```

## 6. Process Management
```javascript
1. ps aux
Displays active processes

2. top	
Displays real-time process usage

3. htop	
Interactive process viewer

4. kill 1234
Kills a process by PID	

5. pkill firefox
Kills a process by name	

6. nice -n 10 myscript.sh
Starts a process with a priority

7. renice 5 -p 2345
Changes priority of a running process	
```


## 7. User Management
```javascript
1. whoami
Displays the current user

2. id username
Shows user and group ID

3. who	
Lists logged-in users

4. w
Shows logged-in users and their processes

5. su username
Switches to another user

6. sudo apt update
Runs commands as root

7. sudo useradd -m newuser
Creates a new user	

8. passwd newuser
Changes user password

9. usermod -aG sudo newuser
Modifies user details

10. sudo deluser newuser
Deletes a user
```



## 8. Package Management
```javascript
1. apt ->	Debian-based package manager -> sudo apt install vim

2. yum ->   RHEL-based package manager -> sudo yum install nano

3. dnf ->   Fedora package manager	->  sudo dnf install tree

4. pacman ->	Arch Linux package manager	->  sudo pacman -S htop
```



## 9. Networking Commands
```javascript
1. ip a
Displays network interfaces	

2. ifconfig	
Shows IP and network details

3. ping google.com
ping	Checks network connectivity

4. netstat -tulnp
netstat	Shows network connections

5. wget <url>
Downloads files from the web

```