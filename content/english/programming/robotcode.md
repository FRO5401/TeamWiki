---
title: "Build and Deploy Robot Code"
meta_title: ""
description: ""
image: "/images/robode.PNG"
categories: ["Programming"]
draft: false
---

Forword\
As part of our development strategy, we must regularly build & deploy code from our computers to our robot. One of the biggest things to keep in mind is that the branch of code you are getting ready to build is fully up to date. If you are trying to deploy the current "master" do the following:

Ensure all your work is saved, committed, and pushed to GitHub

Open GitHub Desktop
Ensure the Current repository in the upper left is set to the name of the current year's game (Ex. ChargedUp2023, Crescendo2024)
Check the Current branch is set to "main" or "master"
Click the Fetch Origin button next to Current Branch
Click Repository from the top bar
Then click Pull
Open WPI VS Code
Checking Jimmy & Ace about performing a rebase

Building & Deploying
After ensuring your code is up to date & rebased. Open WPI VS Code & after the Java checks at the bottom finish, perform the following.

1. Open Command Pallet by pressing Ctrl + Shift + P  2. Search for Build Robot Code & select the option below  There is a chance nothing will happen for a few seconds depending on how old your laptop might be, as long as the bottom right of VS shows Java with a circling wheel, you are fine

3. Look in the terminal for a Build Successful 

4. Ensure the Robot is connected either by USB to the RoboRio or via Wifi to the Radio.

5. Then look in Command Pallet for Deploy Robot Code & select it. Wait for Build Successful to appear. If you receive a build failed, re-run the Build Robot Code again.