#### Description of kali 
```cat /etc/os-release```
#### To know ip addr with specific adaptor
```ip addr | grep eth0```
#### Install nmap
```sudo apt install nmap```
#### To check the opened port of a device/server
```sudo nmap -sS -A --open --top-ports 500 ip_address```
#### To find the ip address 
old command ```ifconfig```
new command ```ip add```
# Learn about telnet
### To run gui of kali with wsl2 install the following
```
sudo apt update && sudo apt -y upgrade
sudo apt install xrdp 
sudo apt install xfce4 xfce4-goodies
sudo apt install dbus-x11
sudo cp /etc/xrdp/xrdp.ini /etc/xrdp/xrdp.ini.bak =>backup of xrdp conf file
sudo sed -i 's/3389/3390/g' /etc/xrdp/xrdp.ini =>changing the default port from 3389 to 3390 so that we can rdp on port 3390
sudo sed -i 's/max_bpp=32/#max_bpp=32\nmax_bpp=128/g' /etc/xrdp/xrdp.ini =>incresing resolution by increasing the bitsPerPixel(bpp)
sudo sed -i 's/xserverbpp=24/#xserverbpp=24\nxserverbpp=128/g' /etc/xrdp/xrdp.ini =>allowing the quality session of rdp to better
echo xfce4-session > ~/xsession =>save this conf to xsession
sudo nano /etc/xrdp/startwm.sh =>to edit the xrdp starting script
comment out last two lines
test -x /etc/X11/Xsession && exec /etc/X11/Xsession
exec /bin/sh /etc/X11/Xsession
add two new lines
# xfce
startxfce4

sudo /etc/init.d/xrdp start => This will start rdp service (Remote Desktop Service)
```


### now run windows serch for remote desktop connection
fill the credential good to go
### i'm sorry lads this was for old kali like of 2020 we are in 2024 so lets find out
---
## wait now the kali desk is more power full and easy
```sudo apt install -y kali-win-kex``` 
that's it F8 to exit the full screen mode good to go