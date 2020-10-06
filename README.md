# Lab2

The purpose of this script is to backup all the pictures on my laptop.

It counts the number of files & folders before & after the backup to ensure no errors.

Since the script is running on Windows via Gitbash, the syntax for paths has to be spelled out.

for ex:  In Linux, the paths would be "tar -czf /tmp/myPics_directory.tar.gz /Users/casey/Pictures"; however, it windows the paths need to include c
"tar -czf /c/tmp/myPics_directory.tar.gz /c/Users/casey/Pictures"

The script uses the following variables:
input=/c/Users/${user}/Pictures
output=/c/tmp/${user}_home_$(date +%Y-%m-%d_%H%M%S).tar.gz

The output filename will include the user name and a formatted date/time. i.e;casey_home_2020-10-04_121818.tar.gz

The script has functions to count the number of files/folder in the source before copying and also after copying.
If the source and tar file numbers match the script will display "Backup of $input completed!" otherwise it will display "Backup of $input failed!"

The script will also display details about the compressed backup 
i.e.; Details about the output backup file:
-rw-r--r-- 1 casey 197609 84352074 Oct  4 12:18 /c/tmp/casey_home_2020-10-04_121818.tar.gz

How to run the script: 
Ensure you have a folder called tmp at the root of your C drive;
type "./PicBackup.sh" 

Email link sent to partner 10/4 1:11 PM.
Link received 10/3 10:40 AM.
