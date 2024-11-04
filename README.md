# OpenScanZero
The cheapest OpenScan Zero 3D scanner project (Mini/Midi)

The title is true if you have a mini milling machine and a Raspberry Zero 2W ;-)
Raspberry zero differs in minimal configuration, so I got rid of the optional connector in my scanner.
The advantages of the project are a lower price and no problems with the camera.

Equipment:

3D-Printer, for example Anet A8 or Prusa I3 (any FDM with 200x200mm print area)
Mini milling machine (i use CNC 1610)
Soldering iron and solder
Tester

Materials:

coPET/PET-g filamet (depends to project type up to 500 grams)
one-sided foiled fiberglass for PCB - two plates 90x70mm or one with similar area.
Raspbery Zero 2W with 16+ Gb microSD card 
IMX519 or Raspberre camera V3 with cable for RasPi Zero. 
two a4988 drivers
two 100uF 16v & two 100nF capacitors
two IRLZ34/IRLZ44 mosfet (you need to cut-off heatsink on it)
two curved pin Header male, 4p, 2.54
LM7805 or better step-down 5V 1A replacement
Pin Header female, 2x20p, 2.54
Barrel Connector, 5.5-2.1mm

two NEMA-17 stepper motor with 50-sm. wires

Eight 1W-led
two resistors 1 ohm
three 26AWG 20sm.-lenght wire 

Varnish for PCB (I have clear)

12V 2A Power Supply

Resources:

You need to download & print scanner parts from https://github.com/OpenScan-org/OpenScan-Design
!!!!!One more thing is needed - a Zero shield holder - just from here - file Mount.stl

Download OpenScan Composer software and firmware from https://www.openscancomposer.com/
Flashing and install manual you can find on that site too.

Development:

Download pcb models 4 OpenScan Zero shield & RingLight just from here - files OpenScanZero.GBR & RingLight.GBR
Mill it ( present modells in Gerber mirrored format) - i use FlatCam for processing and Candle for milling

3. Drill the mounting holes in the RingLight board with a 4mm drill and the central hole for the camera 16mm
4. Solder LEDs and resistors on it. Observe the polarity - there are two groups of LEDs in series.
5. Check the functionality of the LEDs by connecting red to +12V and green, blue to minus. Cover the board with varnish.

6. Solder the power connector and jumpers to the shield board
7. Solder capacitors, connectors and transistors. They should not touch the jumpers
8. Solder the stepper motor drivers & Pin Header female.
9. Connect the power supply. Did the smoke not go away? Perfectly! Adjust the current of the a4988 drivers.
10. Solder the connectors on the Raspberry pi with the pins facing down. Insert the microSD firmware into the Raspberry and its into the shield.
11.  Still no smoke and the LEDs flashed a few times? Great! Print plastic parts!
12. The compilation process is described at https://openscan-org.github.io/OpenScan-Doc/

The camera is fixed with double-sided tape. OpenScan shield is attached with glue.

Yes, the system is far from ideal, but it worked for me the first time


