---
layout: post
title:  "Arduino based waterproof GPS logger"
categories: openstreetmap gps hardware electronics arduino
---

The Shenzen based open hardware company [Seeed Studio](http://www.seeedstudio.com/) offers two products called "[Seeeduino Stalker - Waterproof Solar Kit](http://www.seeedstudio.com/depot/seeeduino-stalker-waterproof-solar-kit-p-911.html)" and "[GPS Bee kit](http://www.seeedstudio.com/depot/gps-bee-kit-with-mini-embedded-antenna-p-560.html)".
This is a great solution if you do not want to design and build your own electronics and waterproof case. The schematics and Eagle design files are available if you would like to build a modified version later.

I got the [Seeeduino Stalker v2.1](http://www.seeedstudio.com/wiki/Seeeduino_Stalker_v2.1), featuring
* an ATmega328P 8-bit Microcontroller, which can be programmed using the Arduino IDE,
* a charging controller, solar cell and battery connectors,
* RTC (and RTC battery holder) for accurate timing and interrupts,
* temperature sensor,
* MicroSD slot,
* [Bee series](http://www.seeedstudio.com/wiki/Bee_series) socket for the [GPS bee](http://www.seeedstudio.com/wiki/GPS_Bee_kit).

The USB to serial bridge present on Arduinos is available on a separate board called [UartSBee](http://www.seeedstudio.com/wiki/UartSBee_V4). It is included in the kit. If you plan to use some of the pin headers, make sure the pin is not used for other functionality already.
The Seeduino Stalker runs on 3.3V and does not work with shields expecting 5V signals. One exception is I2C, read the [wiki page](http://www.seeedstudio.com/wiki/Seeeduino_Stalker_v2.1) for details.

My GPS bee came with a u-blox NEO-6M module.


## Uploading sketches

In the Arduino IDE, select Tools, Board, Arduino Pro or Pro Mini (3.3V, 8MHz) w/ ATmega 328.
