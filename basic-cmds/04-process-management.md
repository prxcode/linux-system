# Process Management Commands  
A Simple commands list for linux.

Note:  
- `PID` = Process ID  
- `sudo` = root/admin privilege  
- Use `man <command>` to see full manual for any command  



## 1. Viewing Running Processes

- `ps` : Show current user's running processes  
- `ps aux` : Show all running processes (detailed view)  
- `ps -ef` : Another format to view all processes  
- `top` : Real-time dynamic process viewer  
- `htop` : Enhanced interactive version of `top` (needs install)  
- `pgrep <name>` : Find PID(s) by process name  
- `pstree` : Show process tree hierarchy  



## 2. Managing (Killing) Processes

- `kill <PID>` : Gracefully stop a process  
- `kill -9 <PID>` : Force kill a process  
- `killall <name>` : Kill all processes by name  
- `pkill <pattern>` : Kill processes matching name or pattern  



## 3. Process Priority Control

- `nice -n <priority> <command>` : Start a process with custom priority  
    - Lower value = higher priority (range: -20 to 19)  
- `renice <priority> -p <PID>` : Change priority of running process  



## 4. Background and Foreground Jobs

- `<command> &` : Start a process in the background  
- `jobs` : View background jobs in current shell  
- `fg %<job_id>` : Bring background job to foreground  
- `bg %<job_id>` : Resume suspended job in background  
- `Ctrl + Z` : Suspend current foreground process  



## 5. Monitoring and Performance Tools

- `watch <command>` : Re-run command repeatedly (default: every 2 seconds)  
  - e.g. `watch -n 1 free -m`  
- `uptime` : Show how long system has been running  
- `vmstat` : Show memory, I/O, and CPU usage  
- `iostat` : Show disk I/O stats (install `sysstat` if missing)  
- `pidstat` : Per-process performance stats  
- `lsof` : List open files and which process is using them  
- `strace -p <PID>` : Trace system calls made by a process  



## 6. Useful Optional Tools (Need Install)

- `htop` : Enhanced real-time system monitor  
- `glances` : Full system performance overview  
- `atop` : Advanced process and system monitor  
- `systemd-cgtop` : Resource usage by control groups  



Note:
- Use `sudo` if access is denied (for system-level processes).
- Combine with `grep` to filter results, e.g. `ps aux | grep firefox`.
- Learn `htop` or `glances` for easier monitoring.

