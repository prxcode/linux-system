# User and Group Management Commands  
A Simple commands list for linux.


## 1. User Management

- `whoami` : Show current logged-in username  
- `id <username>` : Show UID, GID, and groups for user  
- `adduser <username>` : Create a new user (interactive)  
- `useradd <username>` : Create a new user (non-interactive, requires config)  
- `passwd <username>` : Set or change password for user  
- `deluser <username>` : Delete user (keeps home dir unless `--remove-home` is used)  
- `usermod -l <newname> <oldname>` : Rename user  
- `usermod -aG <group> <username>` : Add user to a group (append)  
- `su <username>` : Switch to another user  
- `sudo -i` : Switch to root user (interactive shell)  
- `chage -l <username>` : List password aging and expiration info  



## 2. Group Management

- `groupadd <groupname>` : Create new group  
- `groupdel <groupname>` : Delete a group  
- `groupmod -n <newname> <oldname>` : Rename a group  
- `groups <username>` : Show groups for a user  
- `gpasswd -a <user> <group>` : Add user to group  
- `gpasswd -d <user> <group>` : Remove user from group  
- `newgrp <group>` : Log in to a new group temporarily (requires relogin for effect)



## 3. Default Files and Locations

- `/etc/passwd` : User account info  
- `/etc/shadow` : Secure user password info (hashed)  
- `/etc/group` : Group info  
- `/etc/gshadow` : Secure group info  
- `/home/<username>/` : Default home directory of user  



## 4. Sudo Management (Admin Rights)

- `sudo <command>` : Run command as root (admin)  
- `visudo` : Safely edit sudo permissions file  
- `sudo usermod -aG sudo <username>` : Add user to sudo (admin) group  
- `sudo deluser <username> sudo` : Remove user from sudo group  

Note: On some systems, the admin group may be called `wheel` instead of `sudo`.



## Common Scenarios
`sudo su -` : to go to sudo mode
- **Create a user and give admin rights:**  
  ```bash
  sudo adduser john  
  sudo usermod -aG sudo john  
