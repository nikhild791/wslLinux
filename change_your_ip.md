## How to change ip automatically
* we are using linux
``` 
sudo apt update
sudo apt install tor
sudo systemctl start tor
sudo systemctl status tor
sudo apt install python3-pip
sudo pip install tornet
sudo tornet --interval 3 --count 0 
interval== after how many seconds you want to change your ip
count == how many times you want to change ip 0 is infinite
```