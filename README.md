# Illuminated advertisement prototype using a TFT-screen

This is illuminated advertisement prototype, using ATmega2560 (Arduino Mega) micro-controller, TFT-screen and EEPROM memory.
On the screen text is rolling from bottom to top, each word on its own line. For testing purposes, PC is connected to the system
using a USB-TTL-cable to input the text.

## Main parts used
- ATmega 2560 (Arduino Mega)
- 128x160 pixel TFT-screen
- 25C320 EEPROM

## Schematic
![schematic](https://github.com/Neoni92/TFT-screen-arduino/blob/master/Schematics/TFT_schematic.png)

## How it works
It is programmed in C and Atmel Studio 7 is used as the development environment. The input text for the TFT-screen is written from
the PC terminal and the PC is connected to the system using a USB-TTL-cable. ATmega 2560 micro-controller saves the input text
to the SPI-connected EEPROM memory. After startup, the text that was last programmed, is read from the memory and shown
automatically again on the screen, rolling from bottom to top, each word on its own line. 
