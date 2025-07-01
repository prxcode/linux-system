# Permissions and Ownership Commands
A Simple commands list for linux.

Note: sudo = admin = owner
w = write, x = execute, r = read

## 1. Viewing Permissions & Ownership
- `ls -l` : List files with permissions, owner and group
- `stat <filename>` : Detailed file info including permission, owner, access times
- `id` : Show current userID and groupIDs
- `whoami` : Show current username

## 2. Changing Permissions
- `chmod 755 <filename>` : Set read/write/execute for ownder, read/execute only for group and others
- `chmod +x <filename>` : Add execute permission to the file
- `chmod -x <filename>` : Remove execute permission to the file
- `chmod u+x <filename>` : Add execute permission for sudo
- `chmod g-x <filename>` : Remove write permission from group

## 3. Changing Ownership
- `chown <user> <filename>` : Change owner of the file
- `chown <user>:<group> <filename>` : Change both owner and group
- `sudo chown -R <user> <directory>`: Change owner recursively on a directory