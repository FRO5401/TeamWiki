---
title: "Test Case Development"
meta_title: ""
description: ""
image: "/images/testcasedev.png"
categories: ["Programming"]
draft: false
---
**Put a Battery in the Robot**\
Description: The robot needs a charged battery to be plugged in to function.\
Pre-condition: Obtain a charged battery from the Pit.

Steps:
| Step & Direction      | Expected Result   
|--------------------------------------|---------------------------------|
|Bring the battery close to the robot. | The battery should be in a position where you can easily place it where it needs to go.|
|Put the battery in the correct place (provide image)|The battery should fit into the slot and the cords should be close enough to be plugged in.|
|Plug that cords into the slots with the corresponding color (provide image)|The robot should be receiving power from the battery when the switch is pushed in.|

**Obtain a Functional Driver Station**\
Description: In order to run robot code and control the robot, you need a Driver Station (Computer with the Driver Station software)\
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
- Obtain a Functional Driver Station.
- Get a new radio from the Pit.

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
- Put a Battery in the Robot.
- Obtain a Functional Driver Station.

Steps:
| Step & Direction | Expected Result   
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

**Start the Robot**
Description: The robot needs to be turned on to test code.
Pre-condition:
- Put a Battery in the Robot.
- (The robot can’t be broken or incomplete).

Steps: IN NEED OF PICTURES.
|Step & Description      |Expected Result       |
|------------------------|----------------------|
|Push the ON switch in   |The lights on the robot turn on|

**Receiving Communication**\
Description: Get communication between the robot and the laptop through the radio.\
Pre-condition:
- Start the Robot.
- Obtain a Functional Driver Station.
- Provide a Functional Radio for the Robot.
- Image the RoboRIO of the Robot.
- (You can plug in an ethernet cable to the radio instead if setting up a functional radio is not the preferred method).

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Make sure the radio is on.|There should be a network with the radio name displaying in the internet access tab.|
|Open the FRC Driver Station App on your Driver Station.|The Driver Station interface should pop up.|
|Connect to the radio network.|The comms light on the driver station should turn green.|
|(If you want to plug in an ethernet cable) Get an ethernet cable from the Pit.|You should have a working ethernet cable.|
|(If you want to plug in an ethernet cable) Plug the ethernet cable into your Driver Station and the RoboRIO ethernet port or the connected radio’s ethernet port if there is one.|The comms light on the driver station should turn green.|

**Plugging in a Controller**\
Description: Plug in a controller to control the robot with the Driver Station\
Pre-condition: Obtain a Functional Driver Station.

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Get a Xbox controller from the Pit.|You should have an Xbox controller.|
|Open the FRC Driver Station software.|You should see the Driver Station interface.|
|Plug the Xbox controller into your Driver Station.|The joysticks light on the Driver Station should turn green.|

**Deploying Robot Code**\
Description: Deploy the robot code to test it.\
Pre-condition:
- Obtain a Functional Driver Station.
- Start the Robot.
- Getting Comms.

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Open V.S. Code and open the file of your robot code(Get it from your Github if you need to).|You should have your robot code opened in V.S. Code.|
|(Only if you need to use Github) Log into Github.|You should be in your Github account.|
|(Only if you need to use Github) Pull up the repository of the code you want to use.|You should see your repository and the green code button.|
|(Only if you need to use Github) Click code then Download ZIP.|The repository should be downloaded.|
|Get rid of all errors.|You should see the Driver Station interface.|
|Open the FRC Driver Station software.|You should see the Driver Station interface.|
|Build the Robot Code.|The build should be successful.|
|Deploy the Robot Code.|The robot code light on the Driver Station should turn green.|

**Test the TeleOp Controls**\
Make a controller map to signify which buttons should be tested.\
Description: Input joystick controls to test the set values and commands\
Pre-condition:
- Start the Robot.
- Obtain a Functional Driver Station.
- Getting Comms.
- Plugging in a Controller.
- Deploying Robot Code.
- Ensure the controller map (to signify which buttons should be tested) is created.

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Push forward and back in any order.|Robot moves forward/backward at expected speed.|
|Push forward/back and push right or left on the other joystick.|Robot turns in the expected order and at the set speed.|
|Press the buttons that are bounded to TeleOp commands.|All TeleOp commands execute successfully.|

Here is an example of the driver controls that would need to be tested.\
JARED PUT AN IMAGE HERE!!!

Here is an example of the operator controls on a robot with an arm and a claw that would need to be tested.\
JARED PUT AN IMAGE HERE!!!

**Test an Auto**\
Description: Test if an autonomous command functions on the robot.\
Pre-condition:
- Start the Robot.
- Obtain a Functional Driver Station.
- Getting Comms.
- Plugging in a Controller.
- Deploying Robot Code.

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|Switch the mode to Autonomous.|The robot should start performing the auto when you enable it.|
|Enable the robot.|The lights should turn on and the auto should start.|

**Test the Claw**\
Description: If the robot has a claw, this is how you test it with code.\
Pre-condition:
- Start the Robot.
- Obtain a Functional Driver Station.
- Getting Comms.
- Plugging in a Controller.
- Deploying Robot Code.

Steps:
| Step & Direction      | Expected Result   
|--------------|-----------|
|The robot code has to be in TeleOp mode.|The orange light should blink and the side lights should turn on.|
|Use the joysticks to move the claw to the game piece.|The robot should be in a position to pick up the game piece.|
|Press the button to extend the claw.|The robot should extend the claw and grab the game piece.|
|Use the joysticks to move the claw to the desired scoring area.|The robot should be in front of the desired scoring area.|
|Press the button to extend the claw and release the game piece.|The game piece should be scored.|
