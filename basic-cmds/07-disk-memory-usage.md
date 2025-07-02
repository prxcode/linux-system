# Disk & Memory Usage Commands  
A Simple commands list for linux.


## 1. Disk Space Usage

- `df -h` : Show disk space in human-readable format (MB/GB)  
- `df -Th` : Show disk space with filesystem types  
- `du -h` : Show size of current directory (and subdirectories)  
- `du -sh <folder>` : Show total size of specific folder (summary)  
- `du -ah <folder>` : Show size of all files and folders recursively  


## 2. Checking Free and Used Memory (RAM)

- `free -h` : Show RAM and swap usage in human-readable form
- `free -m` : Show in MB (default: kilobytes)
- `cat /proc/meminfo` : Detailed RAM information



## 3. Top Tools for Monitoring Usage

- `top` : Real-time view of CPU, RAM, and processes
- `htop` : Enhanced `top` (requires `sudo apt install htop`)
- `watch free -h` : Live monitor memory usage every 2 seconds



## 4. Filesystem & Partition Information

- `lsblk` : Show block devices (drives, partitions)
- `fdisk -l` : Detailed info about partitions (requires sudo)
- `blkid` : Show block device UUID and type info
- `mount` : Show currently mounted filesystems
- `findmnt` : Tree view of mounted filesystems



## 5. Disk Usage Analysis Tools (Optional Install)

- `ncdu` : Terminal-based disk usage analyzer (`sudo apt install ncdu`)
- `baobab` : GUI disk usage analyzer (for desktop environments)


## 6. Cleaning Up Disk Space

- `sudo apt autoremove` : Remove unused packages
- `sudo apt autoclean` : Clean obsolete cached packages
- `sudo apt clean` : Delete all downloaded package files
- `journalctl --vacuum-time=7d` : Remove system logs older than 7 days



## 7. Swap Memory Management

- `swapon --show` : Show active swap
- `sudo swapon <swapfile>` : Enable swap file
- `sudo swapoff <swapfile>` : Disable swap file
- `free -h` : Check if swap is being used
