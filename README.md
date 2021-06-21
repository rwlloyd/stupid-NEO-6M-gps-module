# Stupid NEO-6M GPS Module

RandomNerd Tutorial

   https://randomnerdtutorials.com/guide-to-neo-6m-gps-module-with-arduino/

How-To from Arduino Create

https://create.arduino.cc/projecthub/ruchir1674/how-to-interface-gps-module-neo-6m-with-arduino-8f90ad

## First things first. 

What comes out of the module? Well, it spits everything out over serial 

running the `getSerialData-gps.ino` will give something along the lines of

    $GPGGA,081325.00,5323.57785,N,00030.84673,W,1,07,1.37,53.8,M,46.5,M,,*7F
    $GPGSA,A,3,29,31,25,26,02,16,12,,,,,,1.89,1.37,1.30*09
    $GPGSV,4,1,13,02,14,036,16,04,14,324,,05,05,088,,09,00,354,*74
    $GPGSV,4,2,13,12,07,102,16,16,10,282,31,18,22,166,15,20,10,083,18*7C
    $GPGSV,4,3,13,25,41,105,21,26,38,286,35,29,77,085,33,31,62,248,36*77
    $GPGSV,4,4,13,33,28,198,29*4A

So, now we know what it does, we need a library to decode, This ^^^

## Download and Installation

TinyGPS++ Library. (Newer than the one found in arduino libraries)

http://arduiniana.org/libraries/tinygpsplus/

To install this library, download from the github repo below, unzip the archive into the Arduino “libraries” folder, and restart Arduino. You should rename the folder “TinyGPSPlus”.

It's github releases. Version at time of writing 1.0.2b

https://github.com/mikalhart/TinyGPSPlus/releases


