## Adafruit TS3USB30 1 to 2 USB Switch PCB

<a href="http://www.adafruit.com/products/5871"><img src="assets/5871.jpg?raw=true" width="500px"><br/>
Click here to purchase one from the Adafruit shop</a>

PCB files for the Adafruit TS3USB30 1 to 2 USB Switch. 

Format is EagleCAD schematic and board layout
* https://www.adafruit.com/product/5871

### Description

The Adafruit TS3USB30 1 to 2 USB Switch is a nifty breakout board for the TI TS3USB30 that will let you connect one of two USB devices to a single port, handy when you have multiple chips that you may want to communicate over USB but you don't want a hub. This breakout will connect one or the other - it's designed specifically for USB so it can handle high bandwidth USB 2.0 connections of 480 Mbps.

Usage is quite simple: there is one 'upstream' connection, use that to connect to the USB Host device like a computer or Host-capable microprocessor. You can use either the USB Type C port or the breakout pads at the bottom. Then connect two different USB peripherals to the power/ground/D+/D- lines on either side. The S pin selects which port is active, low signal is port 1, high signal is port 2. The Output Enable pin lets you disconnect both. 

Note that power is not switched, just data! Both sides will be powered as the switch connects from one to the other. So, you need your peripherals to know when USB data has been disconnected if you want them to act differently or to re-enumerate. We noticed that solid-state chips like FT232's and USB sticks were great about this, but microcontrollers could be confused and not re-enumerate because they only enumerate on power up. In that case, you'll want to also reset the device via it's own Reset or Enable pin.

The breakout board comes fully assembled, with a 3.3V regulator from 5V and a green power LED that can be disabled. Some header is also included if you'd like to use it in a breadboard - you may find you're maxed out at 12 Mbps speeds though. Four mounting holes make it easy to attach anywhere you like. 

### License

Adafruit invests time and resources providing this open source design, please support Adafruit and open-source hardware by purchasing products from [Adafruit](https://www.adafruit.com)!

Designed by Limor Fried/Ladyada for Adafruit Industries.

Creative Commons Attribution/Share-Alike, all text above must be included in any redistribution. 
See license.txt for additional details.
