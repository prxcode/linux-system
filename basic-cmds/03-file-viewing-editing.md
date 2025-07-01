# File Viewing and Editing Commands
A Simple commands list for linux.

Note: sudo = admin = owner
w = write, x = execute, r = read

## 1. Viewing File Contents
- `cat <filename>` : Display entire file content
- `less <filename>` : View full file content page by page (scrollable)
- `more <filename>` : Similar to less, but more page
- `head <filename>` : Show first 10 lines of a file 
- `head -n 20 <filename>` : Show first 20 lines; here n = number of lines, if no not mentioned then it takes n=10
- `tail -n 20 <filename>` : Show first 20 lines; here n = number of lines


## 2. Searching Inside Files
grep is similar to find ctrl + F in windows
- `grep "hello" <filename>` : Search for text pattern inside a file 
- `grep -r "pattern" <directory>/`  : Recursive search inside directory
- `grep -i "pattern" <filename>` : Case-insensitive Search

## 3. Editing Files (Terminal Editors)
- `nano <filename>` : Easy-to-use text editor (beginner friendly)
- `vim <filename>` : Powerful and popular text editor (advanced)
- `vi <filename>` : Older version of vim, available everywhere
- `gedit <filename>` : GUI text editor (on systems with GUI)

Note: I might create a separate list for Vim and Nano text editors as well, kindly check!

## 4. Creating and Overwriting Files
- `echo "text" > <filename>` : Create or overwrite file with text
- `echo "text" >> <filename>` : Append text to the end of a file

## 5. File Permission for Editing
Note: if you don't have root user access type:
- `sudo nano <filename>`
- `sudo vim <filename>`
