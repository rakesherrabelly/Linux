Connecting to machine (Remote Linux Server) using ssh:
SSH means Secure Shell ssh username@server ssh server -1 username
ssh server -1 username -p 2222
ssh 128.199.138.34 -1 root ssh -i "gvn.pem" blah blah
Privacy Enhanced Mail|Certificate| Password

cat /etc/os-release
pwd
1s, la -lart, ll
mkdir
rmdir
rm -rf
touch
echo
clear
date
time
cd
mv a .a
ср
cp -R

\ : negate
ex: touch abc\ def (This will create as a one file 'abc def' because it ignores space)

echo $? : returns exit code of last command execution. If the cmd execution is successfull then output will be 0 if not non-zero code based on error.

head
head -n (-n = number of lines )
tail

grep
wc : prints lineCount wordCount byteCount
-l : prints only line count
-w : prints only word count
-c : prints only byteCount
-m : prints character count

sudo apt-get update -y
sudo apt-get install tree
tree
tree -a folder

id : Print user and group information for each specified USER.
id username

groups : Print group memberships for each USERNAME or, if no USERNAME is specified, for
the current process.

who : Print information about users who are currently logged in.

whoami : Print the user name associated with the current effective user ID

sudo chown username filename
sudo chown -c username filename (-c is to display comment of the command done, like verbose)
sudo chown :groupname filename
sudo chown username:groupname filename
sudo chgrp groupname filename
sudo chgrp -R groupname filename

sudo useradd username : low level command
sudo adduser username

sudo userdel user : low level command
sudo deluser user

sudo groupadd groupname
sudo addgroup groupname

sudo groupdel groupname
sudo delgroup groupname

chmod 777
chmod u+x
UGO
rwx=421

redirection:
who › users
cat users
echo line 1 > users
echo line 2 >> users
| : o/p of one cmd will be i/p of other cmd
head filename | grep text | wc -l
