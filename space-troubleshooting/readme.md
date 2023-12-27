- Find the largest file in a directory and its subdirectories using the find command
command 1 :
```git
 ubuntu@ip-10-0-2-247:~$ find . -printf '%s %p\n'|sort -nr |head -10
````

Command 2 : 
````git
find /path/to/dir/ -printf '%s %p\n'| sort -nr | head -10
````

Command 3:
```git
# another option ##
find /path/to/search/ -type f -iname "*.mp4" -printf '%s %p\n'| sort -nr | head -10
```

- Truncate File to Specific Size
Use the truncate command to reduce a file to a specific size. The default value is in bytes, which has the following syntax-

Syntax:
```git
truncate -s [number of bytes] filename
````
Example : 
````git
truncate -s 10K filename
truncate -s 0 filename
````

- Get the total diskspace utilized
```git 
 df /|grep /|awk -F" " '{print $5}'| sed 's/%//g'

where :
 df /                  =  get all space information about the root directory
grep /                 = filter the record
awk -F" " '{print $5}' =  print column number 5 information filtered by space
sed 's/%//g'           =  remove the % from the output and display the final value 
```
