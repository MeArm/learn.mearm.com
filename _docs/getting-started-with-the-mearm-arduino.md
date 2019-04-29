---
title: Getting started with the Arduino Compatible MeArm Wifi Kit
summary: Here's where to get your MeArm working with Arduino
layout: doc
tags:
  - Guide
  - Build
  - Arduino
hardware: mearm-v3
type: instruction
level: core
---

The MeArm Robot Arduino Compatible or Wifi Kit is a great place to start with your MeArm adventure. This is the easiest way to get started with the MeArm as the controller board comes preprogrammed. This means you just need to power the control board using a USB power supply or battery pack, connect it to the MeArm base board, and connect the servo motors to start the calibration process.

We cover this whole process in the following video, in addition to the written instuctions below.

<iframe width="560" height="315" src="https://www.youtube.com/embed/sPdbs9b5udQ" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Attach the servo motors provided to your MeArm Base Board, matching the Orange wire to the Y (or O on later boards). Connect the MeArm Arduino Compatible Board and MeArm Base Board together using the 6 pin ribbon cable provided.

Power the MeArm Arduino Compatible Board using a 2A+ 5V USB Power Supply or a 6V AA battery pack (both sold separately).

Your Servo Motors should spring to life as the Arduino Compatible board is powered, defaulting to their 90 degree positions. Attach the following servo horns in the following positions.

![](/assets/docs/mearm-microbit-setup/Servoset.png) 

This is the calibration of your servo motors completed. Use them as required in the [MeArm build instructions](https://learn.mime.co.uk/docs/building-the-mearm-v3).

Once assembled you can reprogram your Arduino Compatible Board using the [Arduino IDE](https://www.arduino.cc/en/main/software)

There are some additional steps to follow once downloading the IDE, before you can interact with the board over your USB connection. Follow the instructions on the [ESP8266](http://esp8266.github.io/Arduino/versions/2.3.0/doc/installing.html) page to set up the board manager. Please install version 2.3.0. We are currently working on the latest version.

Download the [Marceu library](https://github.com/mimeindustries/Marceau) and [MeArm libraries](https://github.com/mimeindustries/MeArm-Arduino) from our Github and follow the instructions to expand your control of the device. We understand this is an advanced step, but we are working to make this a more simple process.

Some users have an experienced an issue where you need to reset the ESP8266, this is done by grounding P0. P0 is available on the underside of the Arduino Compatible board.

