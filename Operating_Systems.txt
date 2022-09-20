Unix Tour

1. 
To display current date - date
To know who you are - whoami
Current directory contents - ls
Other logged in users - who or w


2. 
Count number of entries in /etc - ls /etc | wc -w
Count entries containing number - ls | grep *[0-9]*

3.
Store ls output to file - ls >> file.txt
New File with two lines - (echo "first line" && echo "Second Line") >> file2.txt

4.
 <ctrl>+h/<ctrl>+?/backspace - deletes  character
 <ctrl>+w - deletes word 
 <ctrl>+u - deletes line
<ctrl>+s suspends output
<ctrl>+q resumes output and
<ctrl>+c interrupts the cat process

5. 
processes on the machine - ps
processes owned by you - ps | grep < username >

6.
Logout of the session - exit


Unix Filesystem

1. 
Absolute path of your home directory - /home/<username>/

2.
<

3.
cd 
mkdir Unix
cd Unix
mkdir -p report/style
mkdir george text
cd style

Creating same directory structure in /bin will require sudo permission

4.
creates 8 files in the current directory
touch a b c d e f g foobar

5.
cp -r unix/report/style ./unix/new/
rm unix/new/foobar
rmdir wont work as directory has contents hence use (rm -r unix/new)
mv unix/report unix/newReport

6.Using the cd and ls commands, explore the complete file system.

7. display all files in your home directory - ls -all


8. 
ls -s -size in blocks (in addition to bytes)
ls -g - group ownership
ls -l - permission bits

9.
ls /
Without using the long format option (-l) files color coding can be used

10.
cd ~/unix
touch file
ln file filedup1
ln file filedup2
ln file filedup3
echo "something hardlinked" >> filedup1
cat filedup1
cat filedup2
cat file
rm file 
cat filedup1


Line Editors
1.
ed <filename>
inside ed 
press i to insert, insery two lines 
press . and then enter key to go back to command mode
type wq to save and exit

2.
open iChing with ed - ed iChing






