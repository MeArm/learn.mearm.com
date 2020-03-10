---
title: MeArm Maker Technical Details
summary: The MeArm Maker is requires a little more DIY than most MeArms
layout: doc
tags:
  - Maker
  - HAT
hardware: mearm-v3
type: documentation
level: advanced
---

**The MeArm Maker requires a separate control board, such as an Ardunio or Raspberry Pi, that can provide a PWM Signal to control the servos**

Power at 5-6V and around 2-3A needs to be supplied to the servo motors via the 5+ (red) pin. With Ground from the power supply attached to GND. The remaining pins control the servo motors and require a PWN output from a microcontroller. The PWN signal generator needs to be connected to the GND of the power supply to provide the correct reference voltage.


The pinout of the 6 pin connector is:

![Pinout](/assets/docs/mearm-pi-hat-technical-details/pinout2.gif)

This article is a stub and we will add more detail in future.
