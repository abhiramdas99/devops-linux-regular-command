# devops-linux-regular-command
Deveops linux regular troubleshooting command 

## For Loop  in single line
- Print number in sequence 
  ```git
  for i in {1..5};do echo $i ; done
  ```
- Print number in sequence increament by 2
```git
for((i=1;i<=5;i+=2)); do echo $i;done
```
  
## Nexted Loop in single line 
- print i and j value 
```git
for i in {0..2};do for j in {0..3};do echo "outer i is $i and inner j is $j";done;done
```
