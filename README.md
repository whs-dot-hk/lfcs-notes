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
