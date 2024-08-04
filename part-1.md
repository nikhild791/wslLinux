```wsl --help```

#### To see which linux i can install
```wsl --list --online```

#### To install a distro
```wsl --install -d Debian or distro name```

#### To see the version and state of the wsl running variants
```wsl -l -v```

#### To see the running version
```wsl --list --running```


#### To change the version of the running machine
```wsl --set-version Name version eg.1 or 2```

#### To make a default version
```wsl --set-default-version 2```

#### linux command
```
uname -a
lsb_release -a
```
# search command for linux
```find . | grep SEARCHname```

### If you ever get any error related to installing the linux packages
for eg. Package 'python3-pip' has no installation candidate
```sudo apt update``` update the refrences

### To make any linux variant as default use
```wsl --set-default Ubuntu-24.04```
and check with this 
```wsl -l```

### <font color="blue" ><center>🐳 docker 🐋</center> </font>
### We can run docker inside the ubuntu distro of wsl for that we need to install the docker after but there is a plot twist 
```wsl -l``` the default linux distro will only have the docker connection if you want other distros to have the docke r following the command
-> go to dokcer setting inside resource inside wsl  integration
enable the distros you are good to go
now you can run
ubuntu within docker within ubuntu within windows

### To find windows file inside linux
all shits are inside mnt

### to find linux file inside windows file explorer
```explorer.exe .```
now open the desired file with open with code command (visual studio) edit it and the changes are visible inside ubuntu machine
see previously we are opening vs code using ```code .``` command that opens the editor but inside the linux machine which might be slow but this is fast 
### sorry it opens the linux file inside the windows code editor whatever you like you can use it either use explore to open or code .