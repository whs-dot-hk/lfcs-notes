# Question 1
```
:se nu
```
```
:7777m0
```
```
:7000d
```
```
:%s/Earth/Globe/g
```
```
Go
# Paste "Auctores Varii" without quotes
```
# Question 2
```sh
sudo touch /home/student/apps/certscript.sh
sudo chmod a+x /home/student/apps/certscript.sh
```
```txt
#!/bin/sh
whoami
ip route|grep default
```
# Question 3
```sh
sudo apt update
sudo apt install -y tmux
```
# Question 4
```sh
systemctl status rc-local
```
```sh
sudo -i
touch /etc/rc.local
chmod +x /etc/rc.local
```
```txt
#!/bin/sh
echo test >> /test.txt
```
```sh
vim /lib/systemd/system/rc-local.service
```
```txt
[Install]
WantedBy=multi-user.target
```
```sh
systemctl enable rc-local
```
# Question 5
```sh
sudo crontab -e
```
```txt
*/1 * * * * pkill -u root -f scan_filesystem
```
# Question 6
```sh
sudo groupadd computestream
sudo mkdir -p /exam/computestream/
sudo chown :computestream /exam/computestream/
```
# Question 7
```sh
sudo useradd candidate
passwd candidate
```
```sh
sudo EDITOR=vim visudo
```
```txt
candidate       ALL=(ALL:ALL) NOPASSWD:ALL
```
# Question 8
```sh
sudo touch /etc/skel/NEWS
```
# Question 9
```sh
sudo groupadd students
```
# Question 10
```sh
sudo mkdir -p /home/school/
sudo useradd harry -m -d /home/school/harry/ -G students
```
```sh
sudo passwd harry
```
```txt
# /home/school/harry/.profile
export PATH=/home/school/harry/binaries:$PATH
```
# Question 11
```sh
sudo useradd sysadmin -m -d /sysadmin/ -s /bin/zsh
sudo passwd sysadmin
```
```sh
sudo EDITOR=vim visudo
```
```txt
sysadmin        ALL=(ALL:ALL) NOPASSWD:ALL
```
# Question 12
No idea
# Question 13
```sh
sudo passwd projectadmin
sudo usermod projectadmin -d /home/projectadmin
```
# Question 14
```sh
sudo usermod devel -s /bin/bash
```
# Question 15
```sh
grep 2605 /etc/services
```
```txt
# /home/student/port-2605.txt
bgpd
```
```sh
grep -E 'imap3|imaps' /etc/services 
```
```txt
# /home/student/imap-ports.txt
993
```
# Question 16
```sh
sudo mount /dev/xvdf2 /mnt/backup/
sudo tar -xvf /mnt/backup/backup-primary.tar.bz2 -C /opt/
```
# Question 17
Remove the line from `/etc/fstab`
# Question 18
Edit the options of the line to include `ro`
# Question 19
```sh
unzip -l /opt/SAMPLE001.zip
unzip /opt/SAMPLE001.zip
```
```sh
tar cvf /opt/SAMPLE0001.tar /opt/SAMPLE001
```
```sh
bzip2 -k /opt/SAMPLE0001.tar
```
```sh
xz -k /opt/SAMPLE0001.tar
```
# Question 20
```sh
find /srv/SAMPLE002 -executible -exec rm {} +
```
```sh
find /srv/SAMPLE002 -type f -atime +30 -exec rm {} +
```
```sh
find /srv/SAMPLE002 -empty -exec rm -rf {} +
```
