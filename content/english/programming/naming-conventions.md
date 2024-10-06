---
title: "Naming Conventions"
meta_title: ""
description: ""
image: "/images/namtions.png"
categories: ["Programming"]
draft: false
---

This refers to how we expect variables, functions, classes, folders, etc. to be named. As we have discussed in your training, classes must start with a Capital letter, and variables & functions must be in camel case (ex. thisIsWhatCamelCaseShouldLookLike). This section refers to what the actual name of your variables, functions, and classes should be called.

Variable Naming convention
Motors
Drivebase
For tank drive, we typically have 2 or 3 motors inside of the planetary gearbox. Since the gearbox motors all turn at the same speed and direction in the gearbox, we assume they are actually just 1 unit. As such we will never power 1 motor different than the rest so the naming in code for each motor does not matter. In general, follow this example here from Charged Up: rightDrive1, leftDrive3.

Non-Drivebase
For non-drivebase motors, the location & function of them is important. We need to ensure that these names are concise but explain their purpose. Ex. openClawMotor, rotateArmMotor, leftArmRotateMotor, rightArmRotateMotor

|Info to include in variables|
|----------------------------|
|Includes Action             |
|Includes Where it is        |

Convention: actionLocationMotor


Cameras
If the robot comes equipped with cameras naming should indicate WHERE the camera is & WHAT the camera is looking for. For example, driveBaseInfeedCamera or clawBallDetectionCamera

Encoders
For the most part, follow the same name as the motor the encoder is paired with and append Encoder to the end.


- PID Numbering Convention
- JUnit Test naming convention
- Else case