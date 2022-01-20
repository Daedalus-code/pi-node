# Trump-node
Trump Node - RaspberryPi with LCD monitoring

*Build your own TrumpCoin Node/StakeBox on a Raspberry Pi with a nice Display.*

![alt text](https://i.imgur.com/5Wg4jR7.jpg)  

##### All parts together cost around 90-100 USD. 

* Raspberry Pi 3 Model B+ - [raspberrypi.org](https://www.raspberrypi.org/products/raspberry-pi-3-model-b-plus/)
* HyperPixel 4.0" IPS Display for Pi - [amazon](https://www.amazon.co.uk/dp/B07HJ59NP3/)
* SD card (16GB, Class 10) - [amazon](https://www.amazon.co.uk/SanDisk-Ultra-Memory-Class-Black/dp/B0143RTB1E)

### Setup script
``cd && git clone https://github.com/Daedalus-code/trump-node.git``  
``cd trump-node && bash include/install``  
``cp pitrump.conf ../``  
edit pitrump.conf  

### Setup rc.local

edit rc.local  
``sudo nano /etc/rc.local``  
Put this before exit, not after!  
``sleep 10 && sudo -u pi bash /usr/local/bin/pitrump &``  
Save with ctrl+o  

### Setup HyperPixel4

* https://github.com/pimoroni/hyperpixel4

Here's a list of active branches and which Pi/display combination they support:

* [Pi3](https://github.com/pimoroni/hyperpixel4/tree/pi3) - Pi 3B+ and earlier, HyperPixel4 Rectangular
* [Pi4](https://github.com/pimoroni/hyperpixel4/tree/pi4) - Pi 4 & Pi 400, HyperPixel4 Rectangular, use `hyperpixel4-rotate` to rotate once installed
* [Square](https://github.com/pimoroni/hyperpixel4/tree/square) - Pi 3B+ and earlier, HyperPixel4 Square (for boards manufactured 2020 and earlier)
* [Square-Pi4](https://github.com/pimoroni/hyperpixel4/tree/square-pi4)  - Pi 4 & Pi 400, HyperPixel4 Square (for boards manufactured 2020 and earlier)
* [Square-2021](https://github.com/pimoroni/hyperpixel4/tree/square-2021) - Pi 3B+ and earlier, HyperPixel4 Square (for boards manufactured 2021 and later)
* [Square-Pi4-2021](https://github.com/pimoroni/hyperpixel4/tree/square-pi4-2021)  - Pi 4 & Pi 400, HyperPixel4 Square (for boards manufactured 2021 and later)
