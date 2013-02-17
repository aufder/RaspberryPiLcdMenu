RaspberryPiLcdMenu
==================

A menu driven application template for the Adafruit LCD Plates on a Raspberry Pi.

It provides a simple way to navigate a nested set of menus, and run various func
tions.  Included is a way to determine the IP address of the Pi when running hea
dless.  Also, allows the user to select from a large list of choices (using List
Selector), by cycling through letters vertically and horizontally.
It uses an XML file to configure the menu structure, and processes tags to enabl
e different options.
It assumes the user has the LCD Plate from Adafruit already attached.  It is als
o possible to make a quick modification to the LCD libraries to detect if the LC
D is attached before progressing into the app.
You can also launch the Python based application from /etc/init.d using the prov
ided init file.  In that mode, you can launch right into the application without
 keyboard or monitor, yet still determine the IP address, change networks if you
 like, or any other capability you build in.

Written by Alan Aufderheide

GPL v3 license, kindly include text above in any redistribution.
