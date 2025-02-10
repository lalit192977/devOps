```javascript
[lalit192977@lalit-vmwarevirtualplatform devops]$ echo file management
file management
[lalit192977@lalit-vmwarevirtualplatform devops]$ sudo su
[sudo] password for lalit192977: 
[lalit-vmwarevirtualplatform devops]# echo how to create a file with "cat"
how to create a file with cat
[lalit-vmwarevirtualplatform devops]# cat >file
this is the file created using cat command[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# cat file
this is the file created using cat command[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# echo creating file using touch command
creating file using touch command
[lalit-vmwarevirtualplatform devops]# touch file1 file2 file3
[lalit-vmwarevirtualplatform devops]# ls
file  file1  file2  file3
[lalit-vmwarevirtualplatform devops]# cat >file1
file updaped using cat or you can say re-write
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# cat file1
file updaped using cat or you can say re-write
[lalit-vmwarevirtualplatform devops]# cat >>file1
appending to file using cat
[lalit-vmwarevirtualplatform devops]# cat file1
file updaped using cat or you can say re-write
appending to file using cat
[lalit-vmwarevirtualplatform devops]# cat file file2 > all
[lalit-vmwarevirtualplatform devops]# cat all
this is the file created using cat command[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# rm all
[lalit-vmwarevirtualplatform devops]# cat file file1
this is the file created using cat commandfile updaped using cat or you can say re-write
appending to file using cat
[lalit-vmwarevirtualplatform devops]# cat file file1 >all
[lalit-vmwarevirtualplatform devops]# cat all
this is the file created using cat commandfile updaped using cat or you can say re-write
appending to file using cat
[lalit-vmwarevirtualplatform devops]# ls
all  file  file1  file2  file3
[lalit-vmwarevirtualplatform devops]# ls -l
total 12
-rw-r--r-- 1 root root 117 Feb 10 09:35 all
-rw-r--r-- 1 root root  42 Feb 10 09:30 file
-rw-r--r-- 1 root root  75 Feb 10 09:34 file1
-rw-r--r-- 1 root root   0 Feb 10 09:33 file2
-rw-r--r-- 1 root root   0 Feb 10 09:33 file3
[lalit-vmwarevirtualplatform devops]# echo hidden file creation
hidden file creation
[lalit-vmwarevirtualplatform devops]# cat > .hidden
this is the hidden file created using cat and it is not visible to the directory
and also not visible with ls - command
[lalit-vmwarevirtualplatform devops]# lls
bash: lls: command not found
[lalit-vmwarevirtualplatform devops]# ls
all  file  file1  file2  file3
[lalit-vmwarevirtualplatform devops]# ls -a
.  ..  all  file  file1  file2  file3  .hidden
[lalit-vmwarevirtualplatform devops]# echo now this is visible
now this is visible
[lalit-vmwarevirtualplatform devops]# 



[lalit-vmwarevirtualplatform devops]# echo lets see the editors there are two common editors i.e. vi and nano 
lets see the editors there are two common editors i.e. vi and nano
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# echo lets start with vi
lets start with vi
[lalit-vmwarevirtualplatform devops]# vi ediorfile
[lalit-vmwarevirtualplatform devops]# cat editorfile
cat: editorfile: No such file or directory
[lalit-vmwarevirtualplatform devops]# cat ediorfile
this is the editor file
created using vi
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# echo lets try with nano
lets try with nano
[lalit-vmwarevirtualplatform devops]# nano editorfile2
[lalit-vmwarevirtualplatform devops]# cat editorfile2
this is the editor file using nano
lets see.....
[lalit-vmwarevirtualplatform devops]# nano editorfile2
[lalit-vmwarevirtualplatform devops]# cat editorfile2
this is the editor file using nano
to use nano - editor is very simple and easy 
but this may not be present to all the flavour of linux
lets see.....
[lalit-vmwarevirtualplatform devops]# 






[lalit-vmwarevirtualplatform devops]# echo lets play with directory
lets play with directory
[lalit-vmwarevirtualplatform devops]# ls
all  ediorfile  editorfile2  f1  f2  f3  file  file1  file2  file3
[lalit-vmwarevirtualplatform devops]# ls -s
total 20
4 all        4 editorfile2  0 f2  4 file   0 file2
4 ediorfile  0 f1           0 f3  4 file1  0 file3
[lalit-vmwarevirtualplatform devops]# ls -l
total 20
-rw-r--r-- 1 root root 117 Feb 10 09:35 all
-rw-r--r-- 1 root root  41 Feb 10 09:46 ediorfile
-rw-r--r-- 1 root root 151 Feb 10 09:50 editorfile2
-rw-r--r-- 1 root root   0 Feb 10 09:42 f1
-rw-r--r-- 1 root root   0 Feb 10 09:42 f2
-rw-r--r-- 1 root root   0 Feb 10 09:42 f3
-rw-r--r-- 1 root root  42 Feb 10 09:30 file
-rw-r--r-- 1 root root  75 Feb 10 09:34 file1
-rw-r--r-- 1 root root   0 Feb 10 09:33 file2
-rw-r--r-- 1 root root   0 Feb 10 09:33 file3
[lalit-vmwarevirtualplatform devops]# echo there is no directory to this current working directory
there is no directory to this current working directory
[lalit-vmwarevirtualplatform devops]# mkdir dir1
[lalit-vmwarevirtualplatform devops]# echo now create multiple directory
now create multiple directory
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# mkdir dir2 dir3
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# echo creating hierarchy directory
creating hierarchy directory
[lalit-vmwarevirtualplatform devops]# mkdir d1/d2/d3
mkdir: cannot create directory ‘d1/d2/d3’: No such file or directory
[lalit-vmwarevirtualplatform devops]# ls
all   dir2  ediorfile    f1  f3    file1  file3
dir1  dir3  editorfile2  f2  file  file2
[lalit-vmwarevirtualplatform devops]# echo all the directory will have blue color
all the directory will have blue color
[lalit-vmwarevirtualplatform devops]# ls
all   dir2  ediorfile    f1  f3    file1  file3
dir1  dir3  editorfile2  f2  file  file2
[lalit-vmwarevirtualplatform devops]# mkdir /d1/d2/d3
mkdir: cannot create directory ‘/d1/d2/d3’: No such file or directory
[lalit-vmwarevirtualplatform devops]# mkdir -p /d1/d2/d3
[lalit-vmwarevirtualplatform devops]# ls -l
total 32
-rw-r--r-- 1 root root  117 Feb 10 09:35 all
drwxr-xr-x 2 root root 4096 Feb 10 09:53 dir1
drwxr-xr-x 2 root root 4096 Feb 10 09:54 dir2
drwxr-xr-x 2 root root 4096 Feb 10 09:54 dir3
-rw-r--r-- 1 root root   41 Feb 10 09:46 ediorfile
-rw-r--r-- 1 root root  151 Feb 10 09:50 editorfile2
-rw-r--r-- 1 root root    0 Feb 10 09:42 f1
-rw-r--r-- 1 root root    0 Feb 10 09:42 f2
-rw-r--r-- 1 root root    0 Feb 10 09:42 f3
-rw-r--r-- 1 root root   42 Feb 10 09:30 file
-rw-r--r-- 1 root root   75 Feb 10 09:34 file1
-rw-r--r-- 1 root root    0 Feb 10 09:33 file2
-rw-r--r-- 1 root root    0 Feb 10 09:33 file3
[lalit-vmwarevirtualplatform devops]# mkdir -p d1/d2/d3
[lalit-vmwarevirtualplatform devops]# ls -l
total 36
-rw-r--r-- 1 root root  117 Feb 10 09:35 all
drwxr-xr-x 3 root root 4096 Feb 10 09:57 d1
drwxr-xr-x 2 root root 4096 Feb 10 09:53 dir1
drwxr-xr-x 2 root root 4096 Feb 10 09:54 dir2
drwxr-xr-x 2 root root 4096 Feb 10 09:54 dir3
-rw-r--r-- 1 root root   41 Feb 10 09:46 ediorfile
-rw-r--r-- 1 root root  151 Feb 10 09:50 editorfile2
-rw-r--r-- 1 root root    0 Feb 10 09:42 f1
-rw-r--r-- 1 root root    0 Feb 10 09:42 f2
-rw-r--r-- 1 root root    0 Feb 10 09:42 f3
-rw-r--r-- 1 root root   42 Feb 10 09:30 file
-rw-r--r-- 1 root root   75 Feb 10 09:34 file1
-rw-r--r-- 1 root root    0 Feb 10 09:33 file2
-rw-r--r-- 1 root root    0 Feb 10 09:33 file3
[lalit-vmwarevirtualplatform devops]# echo now hierarchy directory is created
now hierarchy directory is created
[lalit-vmwarevirtualplatform devops]# echo lets see the directory structure where we are currently working
lets see the directory structure where we are currently working
[lalit-vmwarevirtualplatform devops]# tree
.
├── all
├── d1
│   └── d2
│       └── d3
├── dir1
├── dir2
├── dir3
├── ediorfile
├── editorfile2
├── f1
├── f2
├── f3
├── file
├── file1
├── file2
└── file3

7 directories, 10 files
[lalit-vmwarevirtualplatform devops]# cd dir1
[lalit-vmwarevirtualplatform dir1]# ls
[lalit-vmwarevirtualplatform dir1]# pwd
/home/lalit192977/Desktop/devops/dir1
[lalit-vmwarevirtualplatform dir1]# 
[lalit-vmwarevirtualplatform dir1]# 
[lalit-vmwarevirtualplatform dir1]# echo make hidden directory
make hidden directory
[lalit-vmwarevirtualplatform dir1]# mkdir .hidden
[lalit-vmwarevirtualplatform dir1]# ls 
[lalit-vmwarevirtualplatform dir1]# ls
[lalit-vmwarevirtualplatform dir1]# ls -l
total 0
[lalit-vmwarevirtualplatform dir1]# ls -a
.  ..  .hidden
[lalit-vmwarevirtualplatform dir1]# echo now you can see the hidden directory
now you can see the hidden directory
[lalit-vmwarevirtualplatform dir1]# 
[lalit-vmwarevirtualplatform dir1]# 
[lalit-vmwarevirtualplatform dir1]# tree
.

0 directories, 0 files
[lalit-vmwarevirtualplatform dir1]# 










[lalit-vmwarevirtualplatform devops]# echo lets play with files and directory
lets play with files and directory
[lalit-vmwarevirtualplatform devops]# ls -l
total 36
-rw-r--r-- 1 root root  117 Feb 10 09:35 all
drwxr-xr-x 3 root root 4096 Feb 10 09:57 d1
drwxr-xr-x 3 root root 4096 Feb 10 10:04 dir1
drwxr-xr-x 2 root root 4096 Feb 10 09:54 dir2
drwxr-xr-x 2 root root 4096 Feb 10 09:54 dir3
-rw-r--r-- 1 root root   41 Feb 10 09:46 ediorfile
-rw-r--r-- 1 root root  151 Feb 10 09:50 editorfile2
-rw-r--r-- 1 root root    0 Feb 10 09:42 f1
-rw-r--r-- 1 root root    0 Feb 10 09:42 f2
-rw-r--r-- 1 root root    0 Feb 10 09:42 f3
-rw-r--r-- 1 root root   42 Feb 10 09:30 file
-rw-r--r-- 1 root root   75 Feb 10 09:34 file1
-rw-r--r-- 1 root root    0 Feb 10 09:33 file2
-rw-r--r-- 1 root root    0 Feb 10 09:33 file3
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# echo remove files
remove files
[lalit-vmwarevirtualplatform devops]# rm f1
[lalit-vmwarevirtualplatform devops]# ls -l
total 36
-rw-r--r-- 1 root root  117 Feb 10 09:35 all
drwxr-xr-x 3 root root 4096 Feb 10 09:57 d1
drwxr-xr-x 3 root root 4096 Feb 10 10:04 dir1
drwxr-xr-x 2 root root 4096 Feb 10 09:54 dir2
drwxr-xr-x 2 root root 4096 Feb 10 09:54 dir3
-rw-r--r-- 1 root root   41 Feb 10 09:46 ediorfile
-rw-r--r-- 1 root root  151 Feb 10 09:50 editorfile2
-rw-r--r-- 1 root root    0 Feb 10 09:42 f2
-rw-r--r-- 1 root root    0 Feb 10 09:42 f3
-rw-r--r-- 1 root root   42 Feb 10 09:30 file
-rw-r--r-- 1 root root   75 Feb 10 09:34 file1
-rw-r--r-- 1 root root    0 Feb 10 09:33 file2
-rw-r--r-- 1 root root    0 Feb 10 09:33 file3
[lalit-vmwarevirtualplatform devops]# rm f2 f3
[lalit-vmwarevirtualplatform devops]# ls
all  d1  dir1  dir2  dir3  ediorfile  editorfile2  file  file1  file2  file3
[lalit-vmwarevirtualplatform devops]# rm ediofile
rm: cannot remove 'ediofile': No such file or directory
[lalit-vmwarevirtualplatform devops]# rm ediorfile
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# rm dir3
rm: cannot remove 'dir3': Is a directory
[lalit-vmwarevirtualplatform devops]# rm file2 file3
[lalit-vmwarevirtualplatform devops]# ls
all  d1  dir1  dir2  dir3  editorfile2  file  file1
[lalit-vmwarevirtualplatform devops]# rmdir dir3
[lalit-vmwarevirtualplatform devops]# ls
all  d1  dir1  dir2  editorfile2  file  file1
[lalit-vmwarevirtualplatform devops]# rm -r dir2
[lalit-vmwarevirtualplatform devops]# tree
.
├── all
├── d1
│   └── d2
│       └── d3
├── dir1
├── editorfile2
├── file
└── file1

5 directories, 4 files
[lalit-vmwarevirtualplatform devops]# echo lets try to remove d1-directory
lets try to remove d1-directory
[lalit-vmwarevirtualplatform devops]# rmdir d1
rmdir: failed to remove 'd1': Directory not empty
[lalit-vmwarevirtualplatform devops]# echo we have to remove it forcefully
we have to remove it forcefully
[lalit-vmwarevirtualplatform devops]# rmdir -r d1
rmdir: invalid option -- 'r'
Try 'rmdir --help' for more information.
[lalit-vmwarevirtualplatform devops]# rmdir -rf d1
rmdir: invalid option -- 'r'
Try 'rmdir --help' for more information.
[lalit-vmwarevirtualplatform devops]# rm -rf d1
[lalit-vmwarevirtualplatform devops]# ls
all  dir1  editorfile2  file  file1
[lalit-vmwarevirtualplatform devops]# tree
.
├── all
├── dir1
├── editorfile2
├── file
└── file1

2 directories, 4 files
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# cat all
this is the file created using cat commandfile updaped using cat or you can say re-write
appending to file using cat
[lalit-vmwarevirtualplatform devops]# cat file
this is the file created using cat command[lalit-vmwarevirtualplatform devops]# nano file
[lalit-vmwarevirtualplatform devops]# cat file
line 1
line2
line3
line4
line5
line6
line7
line8
line9
line10
line11
line12

[lalit-vmwarevirtualplatform devops]# tac file

line12
line11
line10
line9
line8
line7
line6
line5
line4
line3
line2
line 1
[lalit-vmwarevirtualplatform devops]# less file
[lalit-vmwarevirtualplatform devops]# more file
line 1
line2
line3
line4
line5
line6
line7
line8
line9
line10
line11
line12

[lalit-vmwarevirtualplatform devops]# head -4 file
line 1
line2
line3
line4
[lalit-vmwarevirtualplatform devops]# tail -5
file
file
[lalit-vmwarevirtualplatform devops]# file -5 file
file: invalid option -- '5'
Usage: file [-bcCdEhikLlNnprsSvzZ0] [--apple] [--extension] [--mime-encoding]
            [--mime-type] [-e <testname>] [-F <separator>]  [-f <namefile>]
            [-m <magicfiles>] [-P <parameter=value>] [--exclude-quiet]
            <file> ...
       file -C [-m <magicfiles>]
       file [--help]
```
```javascript
[lalit-vmwarevirtualplatform devops]# tail -5 file
line9
line10
line11
line12

[lalit-vmwarevirtualplatform devops]# touch copyfile
[lalit-vmwarevirtualplatform devops]# ls
all  copyfile  dir1  editorfile2  file  file1
[lalit-vmwarevirtualplatform devops]# cp all copyfile
[lalit-vmwarevirtualplatform devops]# cat copyfile
this is the file created using cat commandfile updaped using cat or you can say re-write
appending to file using cat
[lalit-vmwarevirtualplatform devops]# cat editorfile2
this is the editor file using nano
to use nano - editor is very simple and easy 
but this may not be present to all the flavour of linux
lets see.....
[lalit-vmwarevirtualplatform devops]# cp editorfile2,file newfile
cp: cannot stat 'editorfile2,file': No such file or directory
[lalit-vmwarevirtualplatform devops]# touch newfile
[lalit-vmwarevirtualplatform devops]# cp editorfile2,file newfile
cp: cannot stat 'editorfile2,file': No such file or directory
[lalit-vmwarevirtualplatform devops]# cp editorfile2 file newfile
cp: target 'newfile': Not a directory
[lalit-vmwarevirtualplatform devops]# cat editorfile2 file > newfile
[lalit-vmwarevirtualplatform devops]# cat newfile
this is the editor file using nano
to use nano - editor is very simple and easy 
but this may not be present to all the flavour of linux
lets see.....
line 1
line2
line3
line4
line5
line6
line7
line8
line9
line10
line11
line12

[lalit-vmwarevirtualplatform devops]# echo move file into directory
move file into directory
[lalit-vmwarevirtualplatform devops]# tree
.
├── all
├── copyfile
├── dir1
├── editorfile2
├── file
├── file1
└── newfile

2 directories, 6 files
[lalit-vmwarevirtualplatform devops]# mv all dir1
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── dir1
│   └── all
├── editorfile2
├── file
├── file1
└── newfile

2 directories, 6 files
[lalit-vmwarevirtualplatform devops]# mv editorfile2,file dir1
mv: cannot stat 'editorfile2,file': No such file or directory
[lalit-vmwarevirtualplatform devops]# mv editorfile2 file dir1
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── dir1
│   ├── all
│   ├── editorfile2
│   └── file
├── file1
└── newfile

2 directories, 6 files
[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# echo renaming the files and directory
renaming the files and directory
[lalit-vmwarevirtualplatform devops]# mv file1 f1
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── dir1
│   ├── all
│   ├── editorfile2
│   └── file
├── f1
└── newfile

2 directories, 6 files
[lalit-vmwarevirtualplatform devops]# cat newfile >nf
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── dir1
│   ├── all
│   ├── editorfile2
│   └── file
├── f1
├── newfile
└── nf

2 directories, 7 files
[lalit-vmwarevirtualplatform devops]# mv dir1 d1
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── d1
│   ├── all
│   ├── editorfile2
│   └── file
├── f1
├── newfile
└── nf

2 directories, 7 files
[lalit-vmwarevirtualplatform devops]# mv f1 /d1/file1
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── d1
│   ├── all
│   ├── editorfile2
│   └── file
├── newfile
└── nf

2 directories, 6 files
[lalit-vmwarevirtualplatform devops]# cat >f1
the f1 file[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── d1
│   ├── all
│   ├── editorfile2
│   └── file
├── f1
├── newfile
└── nf

2 directories, 7 files
[lalit-vmwarevirtualplatform devops]# rm f1
[lalit-vmwarevirtualplatform devops]# cat >f1.txt
the text file^X^H[lalit-vmwarevirtualplatform devops]# 
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── d1
│   ├── all
│   ├── editorfile2
│   └── file
├── f1.txt
├── newfile
└── nf

2 directories, 7 files
[lalit-vmwarevirtualplatform devops]# mv f1.txt /d1/newtext.txt
[lalit-vmwarevirtualplatform devops]# tree
.
├── copyfile
├── d1
│   ├── all
│   ├── editorfile2
│   └── file
├── newfile
└── nf

2 directories, 6 files
[lalit-vmwarevirtualplatform devops] 





[lalit-vmwarevirtualplatform devops]# echo Compression and Archiving
Compression and Archiving
[lalit-vmwarevirtualplatform devops]# touch file
[lalit-vmwarevirtualplatform devops]# mkdir dir
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
└── file

2 directories, 1 file
[lalit-vmwarevirtualplatform devops]# tar file.tar file
tar: invalid option -- 'e'
Try 'tar --help' or 'tar --usage' for more information.
[lalit-vmwarevirtualplatform devops]# tar -cvf file.tar file
file
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
├── file
└── file.tar

2 directories, 2 files
[lalit-vmwarevirtualplatform devops]# echo lets compress the size
lets compress the size
[lalit-vmwarevirtualplatform devops]# ls -l
total 16
drwxr-xr-x 2 root root  4096 Feb 10 10:53 dir
-rw-r--r-- 1 root root     0 Feb 10 10:53 file
-rw-r--r-- 1 root root 10240 Feb 10 10:56 file.tar
[lalit-vmwarevirtualplatform devops]# gzip file.tar
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
├── file
└── file.tar.gz

2 directories, 2 files
[lalit-vmwarevirtualplatform devops]# ls -l
total 8
drwxr-xr-x 2 root root 4096 Feb 10 10:53 dir
-rw-r--r-- 1 root root    0 Feb 10 10:53 file
-rw-r--r-- 1 root root  119 Feb 10 10:56 file.tar.gz
[lalit-vmwarevirtualplatform devops]# gunzip file.tar.gz
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
├── file
└── file.tar

2 directories, 2 files
[lalit-vmwarevirtualplatform devops]# ls -l
total 16
drwxr-xr-x 2 root root  4096 Feb 10 10:53 dir
-rw-r--r-- 1 root root     0 Feb 10 10:53 file
-rw-r--r-- 1 root root 10240 Feb 10 10:56 file.tar
[lalit-vmwarevirtualplatform devops]# tar -xvf file.tar
file
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
├── file
└── file.tar

2 directories, 2 files
[lalit-vmwarevirtualplatform devops]# rm file
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
└── file.tar

2 directories, 1 file
[lalit-vmwarevirtualplatform devops]# tar -xvf file.tar
file
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
├── file
└── file.tar

2 directories, 2 files
[lalit-vmwarevirtualplatform devops]# rm file file.tar
[lalit-vmwarevirtualplatform devops]# tree
.
└── dir

2 directories, 0 files
[lalit-vmwarevirtualplatform devops]# tar -cvf dir.tar dir
dir/
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
└── dir.tar

2 directories, 1 file
[lalit-vmwarevirtualplatform devops]# rm -rf dir
[lalit-vmwarevirtualplatform devops]# tree
.
└── dir.tar

1 directory, 1 file
[lalit-vmwarevirtualplatform devops]# gzip dir.tar
[lalit-vmwarevirtualplatform devops]# tree
.
└── dir.tar.gz

1 directory, 1 file
[lalit-vmwarevirtualplatform devops]# gunzip dir.tar.gz
[lalit-vmwarevirtualplatform devops]# tree
.
└── dir.tar

1 directory, 1 file
[lalit-vmwarevirtualplatform devops]# tar -xvf tar
tar: tar: Cannot open: No such file or directory
tar: Error is not recoverable: exiting now
[lalit-vmwarevirtualplatform devops]# tar -xvf dir.tar
dir/
[lalit-vmwarevirtualplatform devops]# tree
.
├── dir
└── dir.tar

2 directories, 1 file
[lalit-vmwarevirtualplatform devops]# 






[lalit-vmwarevirtualplatform devops]# whoami
root
[lalit-vmwarevirtualplatform devops]# logname
lalit192977
[lalit-vmwarevirtualplatform devops]# w
 11:27:00 up  2:04,  2 users,  load average: 0.00, 0.00, 0.00
USER     TTY       LOGIN@   IDLE   JCPU   PCPU  WHAT
lalit192           09:25    2:04m  0.00s  0.07s lightdm --session-child 13 20
lalit192           09:25    2:04m  0.00s  0.60s /usr/lib/systemd/systemd --user
[lalit-vmwarevirtualplatform devops]# who
lalit192977 tty7         2025-02-10 09:25 (:0)
lalit192977 pts/1        2025-02-10 09:29
lalit192977 pts/3        2025-02-10 10:00





[lalit-vmwarevirtualplatform devops]# cat /etc/passwd
root:x:0:0::/root:/usr/bin/bash
nobody:x:65534:65534:Kernel Overflow User:/:/usr/bin/nologin
dbus:x:81:81:System Message Bus:/:/usr/bin/nologin
bin:x:1:1::/:/usr/bin/nologin
daemon:x:2:2::/:/usr/bin/nologin
mail:x:8:12::/var/spool/mail:/usr/bin/nologin
ftp:x:14:11::/srv/ftp:/usr/bin/nologin
http:x:33:33::/srv/http:/usr/bin/nologin
systemd-coredump:x:980:980:systemd Core Dumper:/:/usr/bin/nologin
systemd-network:x:979:979:systemd Network Management:/:/usr/bin/nologin
systemd-oom:x:978:978:systemd Userspace OOM Killer:/:/usr/bin/nologin
systemd-journal-remote:x:977:977:systemd Journal Remote:/:/usr/bin/nologin
systemd-resolve:x:976:976:systemd Resolver:/:/usr/bin/nologin
systemd-timesync:x:975:975:systemd Time Synchronization:/:/usr/bin/nologin
tss:x:974:974:tss user for tpm2:/:/usr/bin/nologin
uuidd:x:68:68::/:/usr/bin/nologin
alpm:x:973:973:Manjaro Linux Package Management:/:/usr/bin/nologin
dnsmasq:x:972:972:dnsmasq daemon:/:/usr/bin/nologin
_talkd:x:971:971:User for legacy talkd server:/:/usr/bin/nologin
polkitd:x:102:102:User for polkitd:/:/usr/bin/nologin
rpc:x:32:32:Rpcbind Daemon:/var/lib/rpcbind:/usr/bin/nologin
rpcuser:x:34:34:RPC Service User:/var/lib/nfs:/usr/bin/nologin
avahi:x:969:969:Avahi mDNS/DNS-SD daemon:/:/usr/bin/nologin
colord:x:968:968:Color management daemon:/var/lib/colord:/usr/bin/nologin
cups:x:209:209:cups helper user:/:/usr/bin/nologin
flatpak:x:967:967:Flatpak system helper:/:/usr/bin/nologin
git:x:966:966:git daemon user:/:/usr/bin/git-shell
lightdm:x:965:965:Light Display Manager:/var/lib/lightdm:/usr/bin/nologin
nm-openconnect:x:964:964:NetworkManager OpenConnect:/:/usr/bin/nologin
nm-openvpn:x:963:963:NetworkManager OpenVPN:/:/usr/bin/nologin
ntp:x:87:87:Network Time Protocol:/var/lib/ntp:/bin/false
openvpn:x:962:962:OpenVPN:/:/usr/bin/nologin
rtkit:x:133:133:RealtimeKit:/proc:/usr/bin/nologin
usbmux:x:140:140:usbmux user:/:/usr/bin/nologin
lalit192977:x:1000:1000:Lalit Thakur:/home/lalit192977:/bin/bash
sujit:x:1001:1001::/home/sujit:/usr/bin/bash
manish:x:1002:1002::/home/manish:/usr/bin/bash





[lalit-vmwarevirtualplatform devops]# sudo userdel manish
[lalit-vmwarevirtualplatform devops]# sudo userdel sujit
[lalit-vmwarevirtualplatform devops]# cat /etc/passwd
root:x:0:0::/root:/usr/bin/bash
nobody:x:65534:65534:Kernel Overflow User:/:/usr/bin/nologin
dbus:x:81:81:System Message Bus:/:/usr/bin/nologin
bin:x:1:1::/:/usr/bin/nologin
daemon:x:2:2::/:/usr/bin/nologin
mail:x:8:12::/var/spool/mail:/usr/bin/nologin
ftp:x:14:11::/srv/ftp:/usr/bin/nologin
http:x:33:33::/srv/http:/usr/bin/nologin
systemd-coredump:x:980:980:systemd Core Dumper:/:/usr/bin/nologin
systemd-network:x:979:979:systemd Network Management:/:/usr/bin/nologin
systemd-oom:x:978:978:systemd Userspace OOM Killer:/:/usr/bin/nologin
systemd-journal-remote:x:977:977:systemd Journal Remote:/:/usr/bin/nologin
systemd-resolve:x:976:976:systemd Resolver:/:/usr/bin/nologin
systemd-timesync:x:975:975:systemd Time Synchronization:/:/usr/bin/nologin
tss:x:974:974:tss user for tpm2:/:/usr/bin/nologin
uuidd:x:68:68::/:/usr/bin/nologin
alpm:x:973:973:Manjaro Linux Package Management:/:/usr/bin/nologin
dnsmasq:x:972:972:dnsmasq daemon:/:/usr/bin/nologin
_talkd:x:971:971:User for legacy talkd server:/:/usr/bin/nologin
polkitd:x:102:102:User for polkitd:/:/usr/bin/nologin
rpc:x:32:32:Rpcbind Daemon:/var/lib/rpcbind:/usr/bin/nologin
rpcuser:x:34:34:RPC Service User:/var/lib/nfs:/usr/bin/nologin
avahi:x:969:969:Avahi mDNS/DNS-SD daemon:/:/usr/bin/nologin
colord:x:968:968:Color management daemon:/var/lib/colord:/usr/bin/nologin
cups:x:209:209:cups helper user:/:/usr/bin/nologin
flatpak:x:967:967:Flatpak system helper:/:/usr/bin/nologin
git:x:966:966:git daemon user:/:/usr/bin/git-shell
lightdm:x:965:965:Light Display Manager:/var/lib/lightdm:/usr/bin/nologin
nm-openconnect:x:964:964:NetworkManager OpenConnect:/:/usr/bin/nologin
nm-openvpn:x:963:963:NetworkManager OpenVPN:/:/usr/bin/nologin
ntp:x:87:87:Network Time Protocol:/var/lib/ntp:/bin/false
openvpn:x:962:962:OpenVPN:/:/usr/bin/nologin
rtkit:x:133:133:RealtimeKit:/proc:/usr/bin/nologin
usbmux:x:140:140:usbmux user:/:/usr/bin/nologin
lalit192977:x:1000:1000:Lalit Thakur:/home/lalit192977:/bin/bash



[lalit-vmwarevirtualplatform devops]# sudo useradd manish
[lalit-vmwarevirtualplatform devops]# cat /etc/passwd
root:x:0:0::/root:/usr/bin/bash
nobody:x:65534:65534:Kernel Overflow User:/:/usr/bin/nologin
dbus:x:81:81:System Message Bus:/:/usr/bin/nologin
bin:x:1:1::/:/usr/bin/nologin
daemon:x:2:2::/:/usr/bin/nologin
mail:x:8:12::/var/spool/mail:/usr/bin/nologin
ftp:x:14:11::/srv/ftp:/usr/bin/nologin
http:x:33:33::/srv/http:/usr/bin/nologin
systemd-coredump:x:980:980:systemd Core Dumper:/:/usr/bin/nologin
systemd-network:x:979:979:systemd Network Management:/:/usr/bin/nologin
systemd-oom:x:978:978:systemd Userspace OOM Killer:/:/usr/bin/nologin
systemd-journal-remote:x:977:977:systemd Journal Remote:/:/usr/bin/nologin
systemd-resolve:x:976:976:systemd Resolver:/:/usr/bin/nologin
systemd-timesync:x:975:975:systemd Time Synchronization:/:/usr/bin/nologin
tss:x:974:974:tss user for tpm2:/:/usr/bin/nologin
uuidd:x:68:68::/:/usr/bin/nologin
alpm:x:973:973:Manjaro Linux Package Management:/:/usr/bin/nologin
dnsmasq:x:972:972:dnsmasq daemon:/:/usr/bin/nologin
_talkd:x:971:971:User for legacy talkd server:/:/usr/bin/nologin
polkitd:x:102:102:User for polkitd:/:/usr/bin/nologin
rpc:x:32:32:Rpcbind Daemon:/var/lib/rpcbind:/usr/bin/nologin
rpcuser:x:34:34:RPC Service User:/var/lib/nfs:/usr/bin/nologin
avahi:x:969:969:Avahi mDNS/DNS-SD daemon:/:/usr/bin/nologin
colord:x:968:968:Color management daemon:/var/lib/colord:/usr/bin/nologin
cups:x:209:209:cups helper user:/:/usr/bin/nologin
flatpak:x:967:967:Flatpak system helper:/:/usr/bin/nologin
git:x:966:966:git daemon user:/:/usr/bin/git-shell
lightdm:x:965:965:Light Display Manager:/var/lib/lightdm:/usr/bin/nologin
nm-openconnect:x:964:964:NetworkManager OpenConnect:/:/usr/bin/nologin
nm-openvpn:x:963:963:NetworkManager OpenVPN:/:/usr/bin/nologin
ntp:x:87:87:Network Time Protocol:/var/lib/ntp:/bin/false
openvpn:x:962:962:OpenVPN:/:/usr/bin/nologin
rtkit:x:133:133:RealtimeKit:/proc:/usr/bin/nologin
usbmux:x:140:140:usbmux user:/:/usr/bin/nologin
lalit192977:x:1000:1000:Lalit Thakur:/home/lalit192977:/bin/bash
manish:x:1001:1001::/home/manish:/usr/bin/bash




[lalit-vmwarevirtualplatform devops]# sudo passwd manish
New password: 
Retype new password: 
passwd: password updated successfully
[lalit-vmwarevirtualplatform devops]# sudo useradd sujit
[lalit-vmwarevirtualplatform devops]# sudo passwd sujit
New password: 
Retype new password: 
passwd: password updated successfully


[lalit-vmwarevirtualplatform devops]# ls
[lalit-vmwarevirtualplatform devops]# su manish
[manish@lalit-vmwarevirtualplatform devops]$ logname
lalit192977
[manish@lalit-vmwarevirtualplatform devops]$ whoami
manish
[manish@lalit-vmwarevirtualplatform devops]$ passwd
Changing password for manish.
Current password: 
mapasswd: Authentication failure
passwd: password unchanged


[manish@lalit-vmwarevirtualplatform devops]$ passwd
Changing password for manish.
Current password: 
New password: 
Retype new password: 
passwd: password updated successfully


[manish@lalit-vmwarevirtualplatform devops]$ su lalit192977
Password: 
[lalit192977@lalit-vmwarevirtualplatform devops]$ sudo su
[sudo] password for lalit192977: 
[lalit-vmwarevirtualplatform devops]# sudo groupadd jerry
groupadd: group 'jerry' already exists
[lalit-vmwarevirtualplatform devops]# cat /etc/group
root:x:0:root
nobody:x:65534:
adm:x:999:daemon
wheel:x:998:lalit192977
utmp:x:997:
audio:x:996:
disk:x:995:
input:x:994:
kmem:x:993:
kvm:x:992:
lp:x:991:cups,lalit192977
optical:x:990:
render:x:989:
sgx:x:988:
storage:x:987:
tty:x:5:
uucp:x:986:
video:x:985:
users:x:984:
sys:x:3:bin,lalit192977
mem:x:8:
ftp:x:11:
mail:x:12:
log:x:19:
smmsp:x:25:
proc:x:26:
games:x:50:
lock:x:54:
network:x:90:lalit192977
floppy:x:94:
scanner:x:96:
power:x:98:lalit192977
groups:x:983:
systemd-journal:x:982:
rfkill:x:981:
dbus:x:81:
bin:x:1:daemon
daemon:x:2:bin
http:x:33:
systemd-coredump:x:980:
systemd-network:x:979:
systemd-oom:x:978:
systemd-journal-remote:x:977:
systemd-resolve:x:976:
systemd-timesync:x:975:
tss:x:974:
uuidd:x:68:
alpm:x:973:
dnsmasq:x:972:
_talkd:x:971:
polkitd:x:102:
rpc:x:32:
rpcuser:x:34:
adbusers:x:970:
ntp:x:87:
locate:x:21:
avahi:x:969:
colord:x:968:
cups:x:209:
flatpak:x:967:
git:x:966:
lightdm:x:965:
nm-openconnect:x:964:
nm-openvpn:x:963:
openvpn:x:962:
rtkit:x:133:
usbmux:x:140:
lalit192977:x:1000:
vboxsf:x:109:
jerry:x:1003:
manish:x:1001:
sujit:x:1002:




[lalit-vmwarevirtualplatform devops]# cat /etc/jerry
cat: /etc/jerry: No such file or directory
[lalit-vmwarevirtualplatform devops]# grep jerry
^X^X^C
[lalit-vmwarevirtualplatform devops]# cat /etc/group
root:x:0:root
nobody:x:65534:
adm:x:999:daemon
wheel:x:998:lalit192977
utmp:x:997:
audio:x:996:
disk:x:995:
input:x:994:
kmem:x:993:
kvm:x:992:
lp:x:991:cups,lalit192977
optical:x:990:
render:x:989:
sgx:x:988:
storage:x:987:
tty:x:5:
uucp:x:986:
video:x:985:
users:x:984:
sys:x:3:bin,lalit192977
mem:x:8:
ftp:x:11:
mail:x:12:
log:x:19:
smmsp:x:25:
proc:x:26:
games:x:50:
lock:x:54:
network:x:90:lalit192977
floppy:x:94:
scanner:x:96:
power:x:98:lalit192977
groups:x:983:
systemd-journal:x:982:
rfkill:x:981:
dbus:x:81:
bin:x:1:daemon
daemon:x:2:bin
http:x:33:
systemd-coredump:x:980:
systemd-network:x:979:
systemd-oom:x:978:
systemd-journal-remote:x:977:
systemd-resolve:x:976:
systemd-timesync:x:975:
tss:x:974:
uuidd:x:68:
alpm:x:973:
dnsmasq:x:972:
_talkd:x:971:
polkitd:x:102:
rpc:x:32:
rpcuser:x:34:
adbusers:x:970:
ntp:x:87:
locate:x:21:
avahi:x:969:
colord:x:968:
cups:x:209:
flatpak:x:967:
git:x:966:
lightdm:x:965:
nm-openconnect:x:964:
nm-openvpn:x:963:
openvpn:x:962:
rtkit:x:133:
usbmux:x:140:
lalit192977:x:1000:
vboxsf:x:109:
jerry:x:1003:
manish:x:1001:
sujit:x:1002:




[lalit-vmwarevirtualplatform devops]# gpasswd -a manish jerry
Adding user manish to group jerry
[lalit-vmwarevirtualplatform devops]# cat /etc/group
root:x:0:root
nobody:x:65534:
adm:x:999:daemon
wheel:x:998:lalit192977
utmp:x:997:
audio:x:996:
disk:x:995:
input:x:994:
kmem:x:993:
kvm:x:992:
lp:x:991:cups,lalit192977
optical:x:990:
render:x:989:
sgx:x:988:
storage:x:987:
tty:x:5:
uucp:x:986:
video:x:985:
users:x:984:
sys:x:3:bin,lalit192977
mem:x:8:
ftp:x:11:
mail:x:12:
log:x:19:
smmsp:x:25:
proc:x:26:
games:x:50:
lock:x:54:
network:x:90:lalit192977
floppy:x:94:
scanner:x:96:
power:x:98:lalit192977
groups:x:983:
systemd-journal:x:982:
rfkill:x:981:
dbus:x:81:
bin:x:1:daemon
daemon:x:2:bin
http:x:33:
systemd-coredump:x:980:
systemd-network:x:979:
systemd-oom:x:978:
systemd-journal-remote:x:977:
systemd-resolve:x:976:
systemd-timesync:x:975:
tss:x:974:
uuidd:x:68:
alpm:x:973:
dnsmasq:x:972:
_talkd:x:971:
polkitd:x:102:
rpc:x:32:
rpcuser:x:34:
adbusers:x:970:
ntp:x:87:
locate:x:21:
avahi:x:969:
colord:x:968:
cups:x:209:
flatpak:x:967:
git:x:966:
lightdm:x:965:
nm-openconnect:x:964:
nm-openvpn:x:963:
openvpn:x:962:
rtkit:x:133:
usbmux:x:140:
lalit192977:x:1000:
vboxsf:x:109:
jerry:x:1003:manish
manish:x:1001:
sujit:x:1002:
[lalit-vmwarevirtualplatform devops]# 



[lalit-vmwarevirtualplatform devops]# echo file permission and ownership
file permission and ownership
[lalit-vmwarevirtualplatform devops]# cat >file
this is the main file
[lalit-vmwarevirtualplatform devops]# ls -l
total 4
-rw-r--r-- 1 root root 22 Feb 10 12:06 file
[lalit-vmwarevirtualplatform devops]# chown manish file
[lalit-vmwarevirtualplatform devops]# ls -l
total 4
-rw-r--r-- 1 manish root 22 Feb 10 12:06 file
[lalit-vmwarevirtualplatform devops]# chown root
chown: missing operand after ‘root’
Try 'chown --help' for more information.
[lalit-vmwarevirtualplatform devops]# chown root file
[lalit-vmwarevirtualplatform devops]# ls -l
total 4
-rw-r--r-- 1 root root 22 Feb 10 12:06 file
[lalit-vmwarevirtualplatform devops]# chmod 760 file
[lalit-vmwarevirtualplatform devops]# ls -l
total 4
-rwxrw---- 1 root root 22 Feb 10 12:06 file
[lalit-vmwarevirtualplatform devops]# cat file
this is the main file
[lalit-vmwarevirtualplatform devops]# su manish
[manish@lalit-vmwarevirtualplatform devops]$ ls
file
[manish@lalit-vmwarevirtualplatform devops]$ cat file
cat: file: Permission denied
[manish@lalit-vmwarevirtualplatform devops]$ ls -l
total 4
-rwxrw---- 1 root root 22 Feb 10 12:06 file
[manish@lalit-vmwarevirtualplatform devops]$ su lalit192977
Password: 
[lalit192977@lalit-vmwarevirtualplatform devops]$ sudo su
[sudo] password for lalit192977: 
[lalit-vmwarevirtualplatform devops]# chown manish file
[lalit-vmwarevirtualplatform devops]# ls -l
total 4
-rwxrw---- 1 manish root 22 Feb 10 12:06 file
[lalit-vmwarevirtualplatform devops]# su manish
[manish@lalit-vmwarevirtualplatform devops]$ cat file
this is the main file
[manish@lalit-vmwarevirtualplatform devops]$ chgroup jerry file
bash: chgroup: command not found
[manish@lalit-vmwarevirtualplatform devops]$ chgrp jerry file
[manish@lalit-vmwarevirtualplatform devops]$ su lalit192977
Password: 
[lalit192977@lalit-vmwarevirtualplatform devops]$ sudo su
[sudo] password for lalit192977: 
[lalit-vmwarevirtualplatform devops]# chgrp jerry file
[lalit-vmwarevirtualplatform devops]# ls -l
total 4
-rwxrw---- 1 manish jerry 22 Feb 10 12:06 file
[lalit-vmwarevirtualplatform devops]# su jerry
su: user jerry does not exist or the user entry does not contain all the required fields
[lalit-vmwarevirtualplatform devops]# chmod 764 file
[lalit-vmwarevirtualplatform devops]# ls -l
total 4
-rwxrw-r-- 1 manish jerry 22 Feb 10 12:06 file
[lalit-vmwarevirtualplatform devops]# cat /etc/group
root:x:0:root
nobody:x:65534:
adm:x:999:daemon
wheel:x:998:lalit192977
utmp:x:997:
audio:x:996:
disk:x:995:
input:x:994:
kmem:x:993:
kvm:x:992:
lp:x:991:cups,lalit192977
optical:x:990:
render:x:989:
sgx:x:988:
storage:x:987:
tty:x:5:
uucp:x:986:
video:x:985:
users:x:984:
sys:x:3:bin,lalit192977
mem:x:8:
ftp:x:11:
mail:x:12:
log:x:19:
smmsp:x:25:
proc:x:26:
games:x:50:
lock:x:54:
network:x:90:lalit192977
floppy:x:94:
scanner:x:96:
power:x:98:lalit192977
groups:x:983:
systemd-journal:x:982:
rfkill:x:981:
dbus:x:81:
bin:x:1:daemon
daemon:x:2:bin
http:x:33:
systemd-coredump:x:980:
systemd-network:x:979:
systemd-oom:x:978:
systemd-journal-remote:x:977:
systemd-resolve:x:976:
systemd-timesync:x:975:
tss:x:974:
uuidd:x:68:
alpm:x:973:
dnsmasq:x:972:
_talkd:x:971:
polkitd:x:102:
rpc:x:32:
rpcuser:x:34:
adbusers:x:970:
ntp:x:87:
locate:x:21:
avahi:x:969:
colord:x:968:
cups:x:209:
flatpak:x:967:
git:x:966:
lightdm:x:965:
nm-openconnect:x:964:
nm-openvpn:x:963:
openvpn:x:962:
rtkit:x:133:
usbmux:x:140:
lalit192977:x:1000:
vboxsf:x:109:
jerry:x:1003:manish
manish:x:1001:
sujit:x:1002:
[lalit-vmwarevirtualplatform devops]# gpasswd -a sujit jerry
Adding user sujit to group jerry
[lalit-vmwarevirtualplatform devops]# su sujit
[sujit@lalit-vmwarevirtualplatform devops]$ ls
file
[sujit@lalit-vmwarevirtualplatform devops]$ cat file
this is the main file
[sujit@lalit-vmwarevirtualplatform devops]$ cat >file
this is the file............
[sujit@lalit-vmwarevirtualplatform devops]$ cat file
this is the file............
[sujit@lalit-vmwarevirtualplatform devops]$ ls -l
total 4
-rwxrw-r-- 1 manish jerry 29 Feb 10 12:17 file
[sujit@lalit-vmwarevirtualplatform devops]$ 




```