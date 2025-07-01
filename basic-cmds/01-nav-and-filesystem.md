# Navigation and File System Commands
A Simple commands list for linux.

## 1. Navigation Commands
Note: Directory means Folder 

- `pwd`: Print current working directory
- `cd`: Change directory
- `ls`: List files and directories
- `ls -l`: Long format (permissions, size, etc.)
- `ls -a`: Show hidden files
- `tree`: Show directory structure


## 2. File & Directory Creation
- `touch <filename>` : Create an empty file or update timestamp
- `mkdir <filename>` : Create a new directory (Empty folder)
- `mkdir -p path` : Create a nested directory



## 3. File & Directory Deletion
- `rm <filename>` : Delete a file
- `rm -r <dirname>` : Delete a directory recursively
- `rm -f <filename>` : Force delete 
- `rmdir <dirname>` : Delete an empty directory 

## 4. File Movement & Copying
- `cp <filename1> <filename2>` : Copy file1 to file2
- `cp -r <dirname1> <dirname2>` : Copy directory recursively 
- `mv <oldname> <newname>` : Rename or move file/directory

## 5. Viewing File & Paths
- `<filename> name` : Show file type(binary, image, text etc)
- `stat <filename>` : Display detailed info about the file
- `basename path` : Show filename from full path
- `<dirname> path` : Show directory name from full path
- `realpath <filename>` : Show absolute path to a file

## 6. File system Structure Tools
- `df -h` : Show disk space usage 
- `du -sh <dirname>` : Show total size of directory
- `lsblk` : List block devices 
- `mount` : Mount a filesystem
- `unmount` : Unmount a filesystem
