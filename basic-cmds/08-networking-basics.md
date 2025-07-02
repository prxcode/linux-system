# Networking Basics Commands  
A Simple commands list for linux.



## 1. Check IP & Network Configuration

- `ip a` or `ip addr` : Show IP addresses and interface info  
- `ip r` or `ip route` : Show routing table  
- `hostname` : Show system hostname  
- `hostname -I` : Show IP address only  
- `ifconfig` : Legacy command for IP/network (use `ip a` instead)  
- `nmcli` : NetworkManager CLI (used in GUI-based Kali setups)  



## 2. Test Network Connectivity

- `ping <host>` : Test network connection (e.g., `ping google.com`)  
- `ping -c 4 <host>` : Send 4 ping packets  
- `traceroute <host>` : Show path packets take to reach host  
- `mtr <host>` : Combine `ping` + `traceroute` in real time  
- `netstat -r` : Show kernel routing table (use `ip route` instead)  
- `ss -tuln` : Show listening ports and connections (`netstat` alternative)  



## 3. DNS and Name Resolution

- `nslookup <domain>` : Get DNS records of domain  
- `dig <domain>` : DNS query tool (more advanced than nslookup)  
- `host <domain>` : Simple DNS lookup  
- `cat /etc/resolv.conf` : Show DNS servers in use  



## 4. Network Scanning & Discovery

- `nmap <IP>` : Scan open ports on a host  
- `nmap -sP <network>/24` : Ping scan a subnet  
- `arp -a` : Show ARP table (local IP-to-MAC mapping)  
- `ip neigh` : Show neighbor devices (replacement for `arp`)  



## 5. Downloading and File Transfer

- `wget <url>` : Download a file from the web  
- `curl <url>` : Fetch web data, REST APIs, or download files  
- `scp <file> user@host:/path/` : Copy file to remote machine over SSH  
- `rsync -av <src> <dest>` : Sync files/directories locally or remotely  



## 6. Interface & Connection Management

- `ip link` : List network interfaces  
- `sudo ip link set <iface> up` : Enable interface  
- `sudo ip link set <iface> down` : Disable interface  
- `nmcli dev status` : Show status of all network devices  
- `sudo dhclient <iface>` : Request IP address via DHCP  
- `iwconfig` : Manage wireless interfaces (deprecated, use `iw`)  


## 7. Network Service Troubleshooting

- `ss -tuln` : Show listening ports and open sockets  
- `netstat -anp` : Show all network connections and PIDs  
- `lsof -i` : List open files related to network  
- `systemctl status NetworkManager` : Check network manager status  
- `journalctl -u NetworkManager` : Show logs for NetworkManager  

