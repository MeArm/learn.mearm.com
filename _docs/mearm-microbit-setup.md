---
title: Getting started with the MeArm micro:bit kit (4505 & 4506)
summary: A guide for setting up the MeArm micro:bit kit
layout: doc
tags:
  - Guide
  - Build
  - micro:bit
hardware: mearm-v3
type: instruction
level: core
---

## Required Materials in this Guide

MeArm micro:bit Kit (4505 or 4506) which includes:
- Acrylic Parts (4 x Acrylic Plates)
- Screws, Rubber Feet, and Hex Wrench (Packaged together)
- MeArm micro:bit Board (PCB4503 AKA MeArm Control Board)
- MeArm Base Board (PCB4502)	
- 4 x Metal Gear Servo Motors, Servo Horns, and Screws
- 6 Pin Rainbow Cable
- 4 x AA Battery Pack

Not included *but required*
 - BBC micro:bit microcontroller
 - Small crosshead screwdriver
 - USB Programming Cable (NB some USB Charging Cables do not have a data line)
 - Personal Computer
 - 4 x AA Batteries or a suitable 6V 2A Power Supply

## Calibration of Servo Motors

Attach the MeArm micro:bit Board (PCB4503) to your MeArm base, using the screws provided. Push the plastic thumb caps down onto the joysticks firmly. We will refer to this as the MeArm Control Board from here, so not to confuse it with the BBC micro:bit.

Plug in your BBC micro:bit (sold separately) into the socket on the MeArm Control Board with the LEDs and buttons on the BBC micro:bit facing upwards. As shown the image below.

Attach a micro USB cable (sold separately) to the BBC micro:bit and attach the other end to your personal computer. Download then drag and drop the [following hex code](http://downloads.mearm.com/MeArm/MeArm-microbit.hex) into the BBC micro:bit device using your personal computer. 

![](/assets/docs/mearm-microbit-setup/microbitsetup.jpg)

Attach the servo motors provided to your MeArm Base Board (PCB4502), matching the Orange wire to the Y (or O on later boards). Connect the MeArm Control Board and MeArm Base Board together using the 6 pin ribbon cable provided.

Power the MeArm Control Board using the battery pack included or a 5-6V 2A+ power supply (6V is best, power supplies sold separately). Powering via the battery pack is the best option, as it provides 6V power for the servos. If using a USB power supply make sure you are using the power port on the MeArm Control Board rather than the programming port on the BBC micro:bit.

![](/assets/docs/mearm-microbit-setup/usb.jpg)

Your Servo Motors should spring to life as the BBC micro:bit is powered via the MeArm Control Board, defaulting to their 90 degree positions. Attach the following servo horns in the following positions.

![](/assets/docs/mearm-microbit-setup/Servoset.png)

This is the calibration of your servo motors completed. 

## Building Your MeArm

Click [here](/assets/mearm.pdf) to download the latest instructions for the MeArm v3, which is the only version used for the MeArm micro:bit Kit. 

Additionally, in association with [Kitronik](http://www.kitronik.co.uk), we have produced this set of video instructions:

**Please note the video shows the MeArm Arduino Version. You can skip ahead for the servo calibration step as you have already completed it**

<iframe width="560" height="315" src="https://www.youtube.com/embed/sPdbs9b5udQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Coding with Your MeArm

Once your MeArm is complete you can explore our make code blocks, by either dragging and dropping the hex code you've downloaded into the browser at [makecode.microsoft.org](https://makecode.microsoft.org/#editor) or adding our package from [GitHub](https://github.com/MeArm/pxt-microbit-mearm).

![](/assets/docs/mearm-microbit-setup/Code5.png)

Thank you for following along and supporting MeArm.
