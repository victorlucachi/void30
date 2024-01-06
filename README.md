# VOID30
*A 30% handwired ortholinear keyboard*

![VOID30](https://i.imgur.com/6EY6A57.jpg)

The VOID30 is a 3d printed, handwired, 30% ortholinear keyboard running QMK Firmware on a Pro Micro controller.

I suggest printing the case using a 0.4 mm nozzle, supports are not needed for any of the parts.

You might want/need to use small dabs of hot glue to secure the switches in the plate depending on how well calibrated your printer is (if you're generous with it, it will add to the weight of the keyboard and it might change the feel of it).

Dont overtighten the screws as the posts could break off and the threads might get stripped.

# Handwiring guide

I've also put together a pretty visual handwiring guide for the VOID9, that you can browse over [here](https://victorlucachi.ro/journal/void9-wiring-guide/).

| ![](https://i.imgur.com/01WknB5.jpg) 	| ![](https://i.imgur.com/GMMczAH.jpg) 	| ![](https://i.imgur.com/5NyUoJY.jpg) 	|
|---------------------------------------|---------------------------------------|---------------------------------------|

# Bill Of Materials

* 30 x diodes ([tme.eu](https://www.tme.eu/ro/en/details/1n4148-dio/tht-universal-diodes/diotec-semiconductor/1n4148/)/[aliexpress](https://www.aliexpress.com/item/32729204179.html))
* 30 x Cherry MX style mechanical switches
* 30 x keycaps of choice
* 1 x Pro Micro ([aliexpress](https://www.aliexpress.com/item/32902569443.html))
* 24 AWG (0.2 mm2) wire
* 4 x 8mm bumpons

### Redux
* 8 x M2x3x3.5 OD heat inserts ([aliexpress](https://www.aliexpress.com/item/4000585933306.html?spm=a2g0o.order_list.order_list_main.33.21ef1802vdSNrS))
* 4 x M2x10 Allen head screws ([aliexpress](https://www.aliexpress.com/item/32966941844.html?spm=a2g0o.order_detail.order_detail_item.9.722ff19cyjrixq))
* 4 x M2x6 Countersunk screws ([aliexpress](https://www.aliexpress.com/item/32968097507.html?spm=a2g0o.order_list.order_list_main.32.21ef1802vdSNrS))

### V1
* 4 x M3x10 countersunk screws that go through the top case ([tme.eu](https://www.tme.eu/ro/en/details/b3x10_bn661/bolts/bossard/1250752/)/[aliexpress](https://www.aliexpress.com/item/32968097507.html))
* 4 x M3x10 allen head screws ([tme.eu](https://www.tme.eu/ro/en/details/m3x10_d912-a2/bolts/kraftberg/)/[aliexpress](https://www.aliexpress.com/item/32966941844.html))
* hotglue

# Pin assignment

    ROW0    ROW1    ROW2
    F6      F7      B1
    
    
    COL0    COL1    COL2    COL3    COL4    COL5    COL6    COL7    COL8    COL9
    F5      F4      B5      B4      E6      D7      C6      D4      D0      D1

# QMK Vial Fork

A QMK Vial fork can be found [here](https://github.com/victorlucachi/vial-qmk/tree/dev_void/keyboards/handwired/void30).

Most features are disabled in order for the firmware to fit on the atmega32u4 present on the Pro Micro controllers, but if you want to tinker around with different features or if you're using a different MCU you can enable/disable them to suit your own needs by editing the rules.mk file in the vial keymap folder.

The web version of Vial is available at [vial.rocks](https://vial.rocks/); it runs in supported browsers (Chrome, Edge and Opera) without requiring an installation.

![VOID30 Vial](https://user-images.githubusercontent.com/2669084/198690678-1ba5441c-e6e7-4980-8934-ea4e442520db.png)

# QMK Fork

A fork containing the QMK config files can be found [here](https://github.com/victorlucachi/qmk_firmware/tree/dev_void/keyboards/handwired/void30). Edit them to suit your own needs and build the firmware following the QMK docs.

If you plan on using the VIA configurator dont forget to download the json definitions file linked in this repository.

# ZMK Config Repo

A ZMK config repo for wireless builds can be found [here](https://github.com/fidepus/ZMK-Config-Void30), thanks to [fidepus](https://github.com/victorlucachi/void30/issues/2). The firmware is configured around the [Puchi BLE](https://keycapsss.com/keyboard-parts/mcu-controller/202/puchi-ble-wireless-microcontroller-pro-micro-replacement) controller, but it can be easily adapted to a nice!nano or any other [ZMK supported hardware](https://zmk.dev/docs/hardware#composite).

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).