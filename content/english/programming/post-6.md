---
title: "Test Case Development"
meta_title: ""
description: ""
image: "/images/image-placeholder.png"
categories: ["Programming"]
#author: "Muffin Man"
# tags: ["nextjs", "tailwind"]
draft: false
---
**Put a Battery in the Robot**\
Description: The robot needs a charged battery to be plugged in to function.\
Pre-condition: Obtain a charged battery from the Pit.

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Bring the battery close to the robot.|The battery should be in a position where you can easily place it where it needs to go.|
|Put the battery in the correct place (provide image)|The battery should fit into the slot and the cords should be close enough to be plugged in.|
|Plug that cords into the slots with the corresponding color (provide image)|The robot should be receiving power from the battery when the switch is pushed in.|

**Obtain a Functional Driver Station**\
Description: In order to run robot code and control the robot, you need a Driver Station(Computer with the Driver Station software)\
Pre-condition: Obtain a computer (It can be your own or a random one from robotics).

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Turn on the computer and set it up if it is a new one.|You should be connected to the internet and able to access Microsoft Edge to download the software.|
|Download the current WPI Library and V.S. Code (Select to download the Library and V.S. Code and then all the default options). [WPI Installation Guide](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-2/wpilib-setup.html)|You should be able to open WPI VScode.|
|Download the current FRC Driver Station (Select all the default options and say no to the Linux statement).[FRC Game Tools Download](https://www.ni.com/en/support/downloads/drivers/download.frc-game-tools.html#479842)|You should be able to open the FRC Driver Station.|
|Download [Github](https://github.com) |You should be able to open the Github Desktop App.|
|Get the Github Extension in V.S. Code by opening V.S. Code and going to Source Control.|The Github Extension of V.S. Code should be downloaded, making it easier to make commits.|
|Log into Github.|You should have access to your Github account and repositories.|

**Provide a Functional Radio for the Robot**\
Description: The robot needs a functioning radio to connect to a Driver Station.\
Pre-condition:
- Obtain a Functional Driver Station
- Get a new radio from the Pit

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Download the FRC Radio Configuration Utility software! [Link!](https://docs.wpilib.org/en/stable/docs/zero-to-robot/step-3/radio-programming.html)|You should be able to open the FRC Radio Configuration Utility.|
|Get an ethernet cable from the Pit.|You should have an ethernet cable.|
|Get a radio power brick from the Pit.|You should have a power brick to charge the radio while configuring it.|
|Plug in the new radio to give it a source of power( to a robot or an outlet).|The power light should start blinking.|
|Plug the ethernet cable into the radio and your Driver Station(Use the port that the software tells you to).|The ethernet light should turn on.|
|Open the FRC Radio Configuration Utility.|You should see a pop-up asking you to pick your network interface.|
|Select ethernet as your network interface and press Okay.|You should see the FRC Radio Configuration Utility interface.|
|Enter the team number as 5401 and enter an appropriate robot name.|The team number and name should be entered.|
|Check if the power light is not blinking.|The power light should be solid and not blinking.|
|Load the firmware.|The firmware load should be successful.|
|Press Configure.|The configuration should be successful.|

**Image the RoboRIO of the Robot**\
Description: Image the roboRIO with the latest software\
Pre-condition:
- Put a Battery in the Robot
- Obtain a Functional Driver Station

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Get a USB Type A male to Type B male cable from the Pit.|You should have the cable.|
|Connect a USB cable from the roboRIO USB Device port to the Driver Station.|The RoboRIO and Driver Station should be connected.|
|Open the RoboRIO Imaging Tool(Comes with [FRC Game Tools](https://www.ni.com/en/support/downloads/drivers/download.frc-game-tools.html#479842))|The RoboRIO should pop up in the top left box.|
|Select the RoboRIO in the top left.|You should be able to update the firmware and image the RoboRIO.|
|Enter 5401 in team number.|The team number should be entered.|
|(If you need to update the firmware, do this) Select Update Firmware in the top right pane.|You should be be able to choose firmware files.|
|(If you need to update the firmware, do this) Select the latest firmware file in the box|The latest firmware should be selected.|
|(If you need to update the firmware, do this) Press Update.|The firmware should update.|
|Select Format Target on the right.|You should be able to choose image versions.|
|Select the latest image version in the box.|The latest version should be selected.|
|Click Reformat to begin the imaging process.|The progress bar should go up until it is complete.|

**Start the Robot**\
Description: The robot needs to be turned on to test code.
Pre-condition:
- Put a Battery in the Robot
- (The robot can’t be broken or incomplete)

Steps: IN NEED OF PICTURES.

**Receiving Communication**\
Description: Get communication between the robot and the laptop through the radio.\
Pre-condition:
- Start the Robot
- Obtain a Functional Driver Station
- Provide a Functional Radio for the Robot
- Image the RoboRIO of the Robot
- (You can plug in an ethernet cable to the radio instead if setting up a functional radio is not the preferred method)

