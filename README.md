RaspberryPiLcdMenu
==================

A menu driven application template for the Adafruit LCD Plates on a Raspberry Pi.

It provides a simple way to navigate a nested set of menus, and run various
functions, by pressing the buttons on the Adafruit LCD Plate.  Included is a way
to determine the IP address of the Pi when running
headless.  Also, allows the user to select from a large list of choices (using
List Selector), by cycling through letters vertically and horizontally.
It uses an XML file to configure the menu structure, and processes tags to
enable different options.  XML element support includes:
- folders, for organizing menus.
- widgets, which are really just functions to call in the code.
- run, which allows you to run any command and see the output on the LCD.

It assumes the user has the LCD Plate from Adafruit already attached.  It is
also possible to make a quick modification to the LCD libraries to detect if
the LCD is attached before progressing into the app.  Though with their new updates, not sure how to do that now.
Support is included also to turn on the LCD to different colors. (at least for
the 16x2 positive LCD plate)
You can also launch the Python based application from /etc/init.d using the
provided init file.  In that mode, you can launch right into the application
without keyboard or monitor, yet still determine the IP address, change networks
if you like, or any other capability you build in.  Obviously double check the
content of the provided init file before use.  Also note that once you put it
in init.d, if you don't actually connect the LCD, you may find lots of error
messages.  You may want to test for presence of the LCD before running it.
Included also is an approach to switch networks from the UI, in case you want to
switch between different network layouts if you travel with it.

Some of the canned menu items are functional, but other are place holders to
spawn ideas.  Such as using gphoto2 to trigger DSLR camera operations, or using
raspistill to capture images from the Pi Camera.  Or using the ephem library to
do astronomy calculations.  Or connecting the Pi to your GPS to auto locate.

To get started, put all these files somewhere.  Then obtain the Adafruit LCD
python code.  From that, copy the files from:
Adafruit-Raspberry-Pi-Python-Code/Adafruit_CharLCDPlate/
into the same folder as this code.

Then you should be able to do:
python lcdmenu.py

Enjoy!

===========
Changes:
25-Jan-2014
 - Added support to set date/time
 - Fixed bug to allow backing out of ListSelector
 - Added support for a reboot command

Written by Alan Aufderheide

GPL v3 license, kindly include text above in any redistribution.
