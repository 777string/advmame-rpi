# advmame-rpi
## AdvanceMAME pre-compiled for Raspberry Pi

This repository contains [AdvanceMAME](http://advancemame.sourceforge.net/index.html) Version 1.2 2012-12 pre-compiled for Raspberry Pi, with high optimizations.

This build was made and tested on [Raspbian](http://www.raspbian.org/).

## Details

Building process:

./configure CFLAGS="-O3 -march=armv6 -mfloat-abi=hard -mfpu=vfp"  
make  
make install  

## Version

\# advmame --version  
AdvanceMAME 1.2  
Compiled Jan 27 2013 with gcc-4.7.2

Drivers (in priority order):  
Video: fb sdl none  
Sound: alsa oss sdl none  
Keyboard: event raw sdl none  
Joystick: event raw sdl none  
Mouse: event raw sdl none  

Directories:  
Data: /usr/local/share/advance  

Configuration (in priority order):  
Host configuration file (R): /usr/local/etc/advmame.rc  
Command line (R)  
Home configuration file (RW): /root/.advance/advmame.rc  
Data configuration file (R): /usr/local/share/advance/advmame.rc

