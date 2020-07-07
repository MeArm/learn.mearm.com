---
title: Setting up and calibrating the MeArm micro:bit kit
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

Attach the MeArm micro:bit Board to your MeArm base, using the screws provided. Push the plastic thumb caps down onto the joysticks firmly.

Plug in your BBC micro:bit (sold separately) into the socket on the MeArm Control Board.

Attach a micro USB cable (sold separately) to the BBC micro:bit and drag and drop the [following hex code](http://downloads.mearm.com/MeArm/MeArm-microbit.hex) into the BBC micro:bit device using your PC, chromebook, or Mac (all sold separately). 

![](/assets/docs/mearm-microbit-setup/microbitsetup.jpg)

Attach the servo motors provided to your MeArm Base Board, matching the Orange wire to the Y (or O on later boards). Connect the MeArm micro:bit Board and MeArm Base Board together using the 6 pin ribbon cable provided.

Power the MeArm Control Board using the battery pack included or a 5-6V 2A+ power supply (6V is best, power supplies sold separately). Powering via the battery pack is the best option, as it provides 6V power for the servos. If using a USB power supply make sure you are using the power port on the MeArm Control Board rather than the programming port on the BBC micro:bit.

![](/assers/docs/mearm-microbit-setup/usb.jpg)

Your Servo Motors should spring to life as the BBC micro:bit is powered via the MeArm Control Board, defaulting to their 90 degree positions. Attach the following servo horns in the following positions.

![](/assets/docs/mearm-microbit-setup/Servoset.png)

This is the calibration of your servo motors completed. Use them as required in the [MeArm build instructions](https://learn.mime.co.uk/docs/building-the-mearm-v3).

Once your MeArm is complete you can explore our make code blocks, by either dragging and dropping the hex code you've downloaded into the browser at [makecode.microsoft.org](https://makecode.microsoft.org/#editor) or adding our package from [GitHub](https://github.com/MeArm/pxt-microbit-mearm).

![](/assets/docs/mearm-microbit-setup/Code5.png)


