- Find the largest file in a directory and its subdirectories using the find command
command 1 :
```git
 ubuntu@ip-10-0-2-247:~$ find . -printf '%s %p\n'|sort -nr |head -10
````

Command 2 : 
......git
find /path/to/dir/ -printf '%s %p\n'| sort -nr | head -10
......
