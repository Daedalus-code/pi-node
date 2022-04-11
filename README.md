![GitHub Maintained](https://img.shields.io/badge/Open%20Source-Yes-green)
![GitHub repo size](https://img.shields.io/github/repo-size/daedalus-code/pi-node)
![GitHub last activity](https://img.shields.io/github/last-commit/daedalus-code/pi-node)

# Pi-Node
Crypto RaspberryPi Node - RaspberryPi with LCD monitoring  

*Build your own crypto Node/StakeBox on a Raspberry Pi with a nice Display.*  

![alt text](https://i.imgur.com/jaMLpjK.jpg)  

##### All parts together cost around 90-100 USD.

* Raspberry Pi 3 Model B+ - [raspberrypi.org](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/)
* HyperPixel 4.0" IPS Display for Pi - [amazon](https://www.amazon.co.uk/dp/B07HJ59NP3/)
* SD card (16GB, Class 10) - [amazon](https://www.amazon.co.uk/SanDisk-Ultra-Memory-Class-Black/dp/B0143RTB1E)

### Setup script
``sudo apt-get install git -y``  
``cd && git clone https://github.com/Daedalus-code/pi-node.git``  
``bash pi-node/include/install``  

### Setup rc.local

edit rc.local  
``sudo nano /etc/rc.local``  
Put this before exit, not after!  
``sleep 10 && sudo -u pi bash /usr/local/bin/pinode &``  
Save with ctrl+o  

### Setup Crontab
``crontab -e``  
Put this at bottom  
``*/1 * * * * bash /usr/local/bin/include/pinode/warden``  
Save with ctrl+o  

### Setup display (HyperPixel4)

* https://github.com/pimoroni/hyperpixel4  

### Setup graphs

![alt text](https://i.imgur.com/LFWAnEF.png)  
