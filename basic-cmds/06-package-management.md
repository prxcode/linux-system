# Package Management Commands (APT-Based)  
A Simple commands list for linux.

Note:  
- Use `sudo` before each command for system-level access.  
- Kali uses **APT** (Advanced Package Tool) as the package manager.  



## 1. Updating System & Repositories

- `sudo apt update` : Update package index (from sources list)  
- `sudo apt upgrade` : Upgrade all installed packages  
- `sudo apt full-upgrade` : Upgrade packages and remove old dependencies  
- `sudo apt dist-upgrade` : Same as `full-upgrade`, used interchangeably  
- `sudo apt autoremove` : Remove unused packages (dependencies no longer needed)  
- `sudo apt autoclean` : Remove obsolete `.deb` files in local cache  
- `sudo apt clean` : Delete all cached package files in `/var/cache/apt/archives`  



## 2. Installing Packages

- `sudo apt install <package>` : Install a new package  
- `sudo apt install <pkg1> <pkg2>` : Install multiple packages  
- `sudo apt install ./package.deb` : Install a local `.deb` file (use `dpkg` too)  



## 3. Removing Packages

- `sudo apt remove <package>` : Remove a package (keeps config files)  
- `sudo apt purge <package>` : Remove package + config files  
- `sudo apt autoremove` : Remove unused dependencies (cleanup)  



## 4. Searching for Packages

- `apt search <keyword>` : Search package names and descriptions  
- `apt list --installed` : List all installed packages  
- `apt list <package>` : Show version and info for specific package  
- `dpkg -l | grep <keyword>` : Filter installed packages (alternative)  



## 5. Getting Package Info

- `apt show <package>` : Show package details (version, dependencies, etc.)  
- `dpkg -s <package>` : Show status of installed package  
- `dpkg -L <package>` : List files installed by a package  
- `which <command>` : Show path of installed binary  
- `whereis <command>` : Show all locations for a binary or command  



## 6. Managing `.deb` Files

- `sudo dpkg -i <package>.deb` : Install `.deb` file manually  
- `sudo dpkg -r <package>` : Remove a manually installed package  
- `sudo dpkg -P <package>` : Purge package (including config)  
- `sudo apt -f install` : Fix broken installs/dependencies  



## 7. Useful Tools

- `apt-cache depends <package>` : Show package dependencies  
- `apt-cache rdepends <package>` : Show reverse dependencies  
- `apt-mark hold <package>` : Prevent package from being upgraded  
- `apt-mark unhold <package>` : Allow package upgrades again  



## 8. Editing Sources (Advanced)

- `/etc/apt/sources.list` : Main file listing APT repositories  
- `sudo nano /etc/apt/sources.list` : Edit repo list  
- After changes:  
  ```bash
  sudo apt update
