# VOID30
*A 30% handwired ortholinear keyboard*

![VOID30](https://i.imgur.com/6EY6A57.jpg)

The VOID30 is a 3d printed, handwired, 30% ortholinear keyboard running QMK Firmware on a Pro Micro controller.

I suggest printing the case using a 0.4 mm nozzle, supports are not needed for any of the parts.

You might want/need to use small dabs of hot glue to secure the switches in the plate depending on how well calibrated your printer is(if you're generous with it, it will add to the weight of the keyboard and it might change the feel of it).

Dont overtighten the screws as the posts could break off and the threads might get stripped.

# Bill Of Materials

* 30 diodes (tme.eu [link](https://www.tme.eu/ro/en/details/1n4148-dio/tht-universal-diodes/diotec-semiconductor/1n4148/))
* 30 cherry mx style switches
* 24 AWG (0.2 mm2) wire
* Pro Micro
* 4 M3x10 countersunk screws that go through the top case (tme.eu [link](https://www.tme.eu/ro/en/details/b3x10_bn661/bolts/bossard/1250752/))
* 4 M3x10(13mm overall length, 5.5mm diameter head) allen head screws that go through the bottom plate (tme.eu [link](https://www.tme.eu/ro/en/details/m3x10_d912-a2/bolts/kraftberg/))
* hot glue for securing the pro micro to the bottom case(optional, but recommended)

# Pin assignment

    ROW0    ROW1    ROW2
    F6      F7      B1
    
    
    COL0    COL1    COL2    COL3    COL4    COL5    COL6    COL7    COL8    COL9
    F5      F4      B5      B4      E6      D7      C6      D4      D0      D1

# QMK Fork

A fork containing the QMK config files can be found [here](https://github.com/victorlucachi/qmk_firmware/tree/master/keyboards/handwired/void30). Edit them to suit your own needs and build the firmware following the QMK docs.
