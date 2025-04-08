![GitHub Maintained](https://img.shields.io/badge/Open%20Source-Yes-green)
![GitHub repo size](https://img.shields.io/github/repo-size/daedalus-code/pi-node)
![GitHub last activity](https://img.shields.io/github/last-commit/daedalus-code/pi-node)

# Pi-Node
## FreedomCoin - RaspberryPi Node  

### Spin up a node
``sudo apt-get install git -y``  

``cd && git clone https://github.com/Daedalus-code/pi-node.git``  

``bash pi-node/include/install``  

### Setup rc.local

edit rc.local  
``sudo nano /etc/rc.local``  

Change 'pi' user if needed, put this before exit, not after!  
``sleep 10 && sudo -u pi bash /usr/local/bin/dash &``  

Save with ctrl+o and reboot  

### Trade FREED on XeggeX, NonKYC

[XeggeX](https://xeggex.com?ref=650e9399625501b3b53b1172)  
[NonKYC](https://nonkyc.io?ref=66a730caaee63aa82784b011)  
