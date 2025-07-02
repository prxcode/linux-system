# Text Processing Commands in Linux  
A Simple commands list for linux.


## 1. Viewing and Reading Text

- `cat <file>` : Print entire file content  
- `less <file>` : View file page by page (scrollable, backward/forward)  
- `more <file>` : View file page by page (forward only)  
- `head <file>` : Show first 10 lines  
- `tail <file>` : Show last 10 lines  
- `tail -f <file>` : Follow file in real time (useful for logs)  



## 2. Searching Inside Text

- `grep "pattern" <file>` : Find lines matching pattern  
- `grep -i "pattern" <file>` : Case-insensitive search  
- `grep -r "pattern" <folder>` : Recursive search in directory  
- `grep -v "pattern" <file>` : Show lines that do **not** match pattern  
- `egrep "pattern1|pattern2"` : Extended regex search  



## 3. Sorting and Uniqueness

- `sort <file>` : Sort lines alphabetically  
- `sort -n <file>` : Sort numerically  
- `sort -r <file>` : Reverse sort  
- `uniq <file>` : Remove duplicate lines (only works on sorted data)  
- `uniq -c <file>` : Count occurrences of unique lines  


## 4. Counting

- `wc <file>` : Count lines, words, characters  
- `wc -l <file>` : Count lines only  
- `wc -w <file>` : Count words only  
- `wc -c <file>` : Count characters (bytes)  



## 5. Cutting and Extracting Columns

- `cut -d':' -f1 <file>` : Split by delimiter (e.g., `:`) and extract field  
- `cut -c1-5 <file>` : Extract specific character positions  
- `awk '{print $1}'` : Print first column (space/tab-delimited by default)  
- `awk -F ':' '{print $1}'` : Print first field using `:` as delimiter  



## 6. Substitution and Replacement

- `sed 's/old/new/' <file>` : Replace first match in each line  
- `sed 's/old/new/g' <file>` : Replace all matches in each line  
- `sed -n '5,10p' <file>` : Print lines 5 through 10  
- `awk '{gsub(/old/, "new"); print}'` : Replace globally in awk  



## 7. Combining Files and Text

- `paste file1 file2` : Merge files line by line  
- `join file1 file2` : Join files based on common field (must be sorted)  
- `cat file1 file2 > merged.txt` : Concatenate into one file  



## 8. Advanced Tools

- `tr 'a-z' 'A-Z'` : Translate characters (lowercase to uppercase)  
- `xargs` : Build and execute command lines from input  
- `cut`, `paste`, `awk`, `sed` : Often used together in pipelines  
- `column -t` : Format plain text into aligned table (with tabular input)  
