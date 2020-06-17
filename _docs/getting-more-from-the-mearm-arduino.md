---
title: Getting more from the Arduino Compatible MeArm Wifi Kit and Getting Back to the Default
summary: There are some extra features and software to go with your MeArm Wifi.
layout: doc
tags:
  - Guide
  - Build
  - Arduino
hardware: mearm-v3
type: instruction
level: advanced
---

Thank you for purchasing a MeArm Wifi Kit. This is an upgrade to the MeArm Deluxe Kit as a Wifi Enabled Arduino Compatible controller of the MeArm with joystick controls. 

The MeArm Wifi used a microcontroller called an ESP8266, using open source software from the Arduino company. The MeArm Wifi Board comes pre-installed with basic software so you can control the MeArm robot arm, but this can be upgraded with more programming languages and / reset to its original state using these instructions.

The first stage of the process is to install and set up the open source [Arduino](https://arduino.cc/en/Guide/Introduction) software. It is available to download from [the Arduino website](https://arduino.cc/en/Main/Software). Select your operating system and follow the instructions given to install. This software is called the Arduino IDE, which stands for Integrated Development Environment.

Next we add support for the ESP8266 microcontroller and our own libraries. To do this:

Launch the Arduino IDE and click on "File-> Preferences".

In "Additional Boards Manager URLs" add "http://arduino.esp8266.com/stable/package_esp8266com_index.json" and click on "OK"

Go to "Tools->Board->Boards Manager", type "ESP8266" and install the support package.

Now we add two lots of software, the first is called Marceau and the second is called MeArm.

Go to "Sketch->Include Library->Manage Libraries", type "Marceau" and install the package.

Download the [MeArm library](https://github.com/mimeindustries/MeArm-Arduino/archive/master.zip).

Go to "Sketch->Include Library->Add .ZIP library", locate the zip file and add it to your libraries.

Go to "File->Examples" and scroll all the way down. Select "INCOMPATIBLE->MeArm->MeArm Wifi". The word "INCOMPATIBLE" is a bit worrying but this is due to part of the name of the ZIP file had a "-" character in it. This will go away after the first time you use it.

Go to "Tools->Board->NodeMCU 1.0 (ESP-12E Module)" which will set the board type to the correct board.

Now click the "tick button" in the top left to verify the code. All being well it should compile. If not check that you've not missed any of the steps outlined above. Since we have not yet connected the MeArm to your PC you won't be able to upload the code - we are checking that the software install is correct before we introduce any hardware.

Once you've verified the code, go to "File->Save as" and save "MeArm Wifi", it should save in the Arduino folder in your documents folder.

Connect your MeArm Wifi Board to your PC or Mac via a micro-USB cable and click upload once it recognised the device and assigns it a COM port. You may need to select the COM port within the "Tools->Boards->Port" menu in the IDE.

Once the code has uploaded you will have the latest version of the MeArm software installed. Next we can add some bonus softare so you can learn to code in more languages (or just use your favourite).

To do this we need to add another tool to the Arduino IDE which allows us to add apps to the MeArm Wifi, giving us access to Blockly, Javascript and Python.

Download the latest version of the plugin on [this website](https://github.com/esp8266/arduino-esp8266fs-plugin/release). 

Unzip the contents and place it in the tools folder of your Arduino directory (for most this is in your Documents directory). You may need to create a new folder called "tools". The final path will look something like this:

`home directory\Arduino\tools\ESP8266FS\tool\esp8266fs.jar`

Restart the Arduino IDE by closing and opening the application.

On reopening your MeArm Wifi example you will see a new option under "Tools->ESP8266 Sketch Data Upload"

With your MeArm Wifi Board connected to your computer you will be able to click this new option and sit back while it uploads the contents of the data folder to your ESP8266.

Once this has finished loading you can close your Arduino IDE.

Open your Wifi Networks and you will see a new network named "MeArm-xxxx" where xxxx represents numbers and letters, for example "MeArm-129C". Join this new network. 

Open your web browser and go to local.mearm.com

You can now operate and program your MeArm via the languages shown when you click the four black squares on the top of the screen.

Finally add the MeArm to your wireless network. Click on the black gear logo in the top right corner. Select your network and input your password. Once connected go back to the black gear logo and note down the IP address that has been assigned by your network to the MeArm (eg 192.168.1.15).

Disconnect from the MeArm network and rejoin your wireless network. Open a browser and type the IP address you've just noted down into it. This should take you to the MeArm control panel where you can experiment with coding your MeArm.
