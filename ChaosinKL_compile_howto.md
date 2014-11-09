========================================================
Compiling Marlin for the chaosinkl printer in a nutshell 
========================================================
0. Get a computer running an OS with avr-gcc and avr-libc installed
1. If you are drunk already or if you still need to drive skip to step 5 
2. Get beer
3. Open beer
4. Drink beer
5. Make a new directoy e.g. chaosinklprinter
6. Clone our Marlin inside it: ` cd chaosinklprinter; git clone  https://github.com/ravinrabbid/Marlin.git `
7. Download the arduino 1.0.0 toolchain from http://arduino.cc/en/Main/OldSoftwareReleases
8. Unpack the toolchain into chaosinklprinter. You should have now two subdirectories in it : Marlin and arduino-1.0.
9. Copy chaosinklprinter/Marlin/ArduinoAddons/Arduino_1.x.x/Sanguino and chaosinklprinter/Marlin/ArduinoAddons/Arduino_1.x.x/rambo to choasinklprinter/arduino-1.0/hardware/.
10. Use shell of your choice within any terminal emulator you like to execute ` make ` inside choasinklprinter/Marlin/Marlin/
11. Flash the hex file from chaosinklprinter/Marlin/Marlin/applet/Marlin.hex on the printer
12. Reapply the eeprom config using the gcode from chaosinklprinter/Marlin/eeprom_settings.txt
13. Get an another beer, you've earned it.
