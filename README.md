# This repository is a copy of the official Marlin 2.0.8, with Tronxy X5SA (and variants) pre-configured.

## On the V6 board there is a W25Qxx SPI FLASH and a 24C16 I2C EEPROM
The Marlin/src/gcode/control/M993_M994.cpp update to  
M993   : Backup SPI Flash to SD spiflash.bin file  
M993 I : Backup I2C 24C16 to SD 24c16.bin file  
M994   : Restore SPI Flash from SD spiflash.bin file  
M994 I : Restore I2C 24C16 from SD 24c16.bin file  

## Display on lcd screen the print picture befor start print
The Marlin/src/ltd/tft/ui_490x320.cpp update to display  
use Tronxy Slicer for generate Gcode witch picture  
copy all lines M4010 and incert a the begining of your Gcode  
## BLTOOUCH configuration for CHITU V6 card
Connect BLTOUCH gnd to WIFI connector Pin 1  
Connect BLTOUCH servo to WIFI connector Pin 2  
Connect BLTOUCH 5V power suply to WIFI connector Pin 4  

Connect BLTOUCH gnd out in place of gnd original captor  
Connect BLTOUCH out in place of out original captor  

comment in Configuration.h line #define BLTOUCH_WIFISLOT if you don't use  