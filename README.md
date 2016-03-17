# garage-door-pi
Garage Door Opener Using a Raspberry Pi - Forked from [Chris Driscoll's Original Code](http://www.driscocity.com/idiots-guide-to-a-raspberry-pi-garage-door-opener/)

Differences from Chris Driscoll's version:
* Added a second door sensor
  * Now supports a normal garage door (front) for a car, as well as a side/back door
  * GPIO 18 used for "FRONT DOOR"
  * GPIO 27 used for "BACK DOOR"
* Added a temperature sensor
  * GPIO 4 (Pin 7)
  * Used a 1-Wire DS18B20 temperature sensor, supported by WebIOPi
* Less Doge...because I am boring. :-/

# Screenshot
[Garage Door Pi Screenshot from an iPhone](http://www.techsneeze.com/wp-content/uploads/2016/03/garage-door-pi_screenshot1.png)

![Test](http://www.techsneeze.com/wp-content/uploads/2016/03/garage-door-pi_screenshot1-169x300.png)

# Installation

1. Follow [Chris Driscoll's Guide](http://www.driscocity.com/idiots-guide-to-a-raspberry-pi-garage-door-opener/).
2. Use the files in this repo instead of the HTML files in the guide.  They should otherwise be placed in the same folder. 
3. Add the line below to the `[DEVICES]` section of  `/etc/webiopi/config` : 
```
Garage = DS18B20
```

