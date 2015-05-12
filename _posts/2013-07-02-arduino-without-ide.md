---
layout: post
title:  "Building an Arduino project without using the Arduino IDE"
date:   2013-07-02 10:11:18
categories: arduino
---
The Arduino IDE brings plug and play to microcontroller programming. Open a sketch, select your board in the board menu, and click play to compile and upload.

Sometimes you might want to know what is going on during the [build process](http://arduino.cc/en/Hacking/BuildProcess).
Edit the Arduino [preferences file](http://arduino.cc/en/Hacking/Preferences) and set
`build.verbose` and `upload.verbose` to `true`.

If you would like to use the Arduino bootloader and library with your own editor, things get a bit more complicated.
There are several build options for Arduino projects:

* Makefile
* Scons
* CMake
* *Ino* CLI tool (recommended)

## Makefile
Older versions of Arduino came with a Makefile, located at `hardware/cores/arduino/Makefile`. You may need to reset the Arduino manually, like in this [troubleshooting guide](http://johanneshoff.com/arduino-command-line.html).

Newer versions are creating a Makefile [during the build process](http://www.arduino.cc/en/Main/Documentation).
People started building their own Makefiles, e.g. [Makefile for the DOGS102 Shield](https://code.google.com/p/dogm128/source/browse/libraries/Dogm/examples/SpaceTrash/Makefile.uno_dogs102)

## Scons
If you prefer a Python build tool, there is Scons support with [arscons](https://github.com/suapapa/arscons).

## CMake
There is also CMake support with [arduino-cmake](https://github.com/queezythegreat/arduino-cmake).

## Ino tool
[Ino](http://inotool.org/) is a CLI tool for working with Arduino. Their [quickstart](http://inotool.org/quickstart) should get you up and running.

This tool worked best for us when we needed a quick solution.
