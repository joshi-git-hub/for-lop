# for-lop
#this is a for loop example and in this example we will make find out a specific file for a directory and
#if we get this file program should be exit. 
# so lats start.
-------------------------***-------------
#!/bin/bash
clear
for i in `ls /etc/`
do 
 echo "file name is  = $i"
 if [ $i = "passwd" ] 
 then
 {
 echo "$i file exist"
 break
 }
fi
done

