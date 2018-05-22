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

##I am adding anothere example of for loop on this repo. 
# by this program we can find out  which is directory and which one is a file in a specific Directory.
#!/bin/bash
cd ~ 
for i in * 
do 
if [ -f  $i ]
then
 {
 echo "$i is a file"
 }
 elif [ -d  $i ]
 then
 {
 echo "$i is a directory."
 }
 fi
 done
