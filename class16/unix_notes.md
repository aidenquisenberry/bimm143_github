## Core Unix commands

Most unix commands have super short names, which makes them quick to type but
annoying to learn. Major file system related commands include:

pwd: print working directory
ls: list files and directories
cd: change directory
mkdir: make a new directory
rm: remove files and directories (delete) - BE AWARE OF WHAT YOU ARE DELETING!!!
cp: copy files (source > destination)
mv: move files or directories (basically re-name)
nano: a wee text editor (very basic but always available)

Further Important Commands:
Basics:                    ls, cd, pwd, man, ssh, scp
File Control:              mv, cp, mkdir, rm, |, >
Viewing & Editing Files:   less, head, tail, nano, touch
Misc. Useful:              chmod, 
curl:                      Download filed from web or gtp
wget:                      Download files from the web
tar -zxvf:                 UnTar (unpackage) Tar archive files
gunzip:                    UnZip files
$PATH: 
Power Commands:           grep, sudo, git, R
Process related:          top, ps, kill, Crl-c, Crl-z, bg, fg

## AWS EC@ Instance

Connect to my instance with:

ssh -i ~/Downloads/bimm143_aidenquisenberry.pem ubunto@some_ip_address

Secure Copy files between machines, in this case from our instance to our laptop

scp -i ~/Downloads/bimm143.aidenquisenberry.pem ubuntu@some_ip_address

## Class 17 instance

ssh -i bimm143_aidenquisenberry.pem ubuntu@ec2-35-94-7-32.us-west-2.compute.amazonaws.com

**sets KEY as variable corresponding to file location**
export KEY=~/Downloads/bimm143_aidenquisenberry.pem
**sets SERVER as variable corresponding to instance**
export SERVER=ubuntu@ec2-35-94-7-32.us-west-2.compute.amazonaws.com
**use `$` symbol to call variable**
ssh -i $KEY $SERVER



