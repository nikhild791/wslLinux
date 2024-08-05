#### To see the process running on linux
```htop```
with tree view F5 we can see the whole process are child process of /init process which enables by wsl 
#####  systemctl command will not work by default read the shit
**systemd** does not enabled by default in wsl so we need to do it
```sudo nano /etc/wsl.conf```
```
[boot]
systemd=true
``` 
^O then enter
then wsl --shutdown 
now when you start you will see a change htop
the /sbin/init runs first then the /init and systemd start 
other process are sevices process or deamon process
but what is sbin/init
lets find 
```ls -al /sbin/in``` it is systemd
* [super cool video](https://www.youtube.com/watch?v=__qwqH0C1xg)
let see the services and deamons started by systemd in list
```systemctl --type=service --state=running```