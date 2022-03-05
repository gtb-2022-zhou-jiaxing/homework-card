# homework-card

## Problem 1

md5sum file1 


## Problem 2

diff file1 file2


## Problem 3
```bash
val=`expr $1 % 2`
  
if [[ $val == 1 ]]
then
   echo "odd"
else
   echo "even"
fi
~
```





## Problem 4

```bash
#!/bin/bash

filePath=$PWD'/result.log'

if [[ ! -f "$filePath" ]]
then
	count=0
	touch $filePath
	cho $count > $filePath
else
	echo "file exits"
 	number=$(cat $filePath)
	((number++))
	echo $number
	echo $number > $filePath
 fi
~
```





## Problem 5

```bash
filePath='number.txt'
awk '{s+=$1} END {print s}' $filePath
```
