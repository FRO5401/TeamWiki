---
title: "Command Line Basics"
meta_title: ""
description: "Basic Bash Commands you should become familiar with"
image: /images/bash-logo.jpg
categories: ["Programming"]
draft: false
---

**Basic Bash Commands you should become familiar with**

# Why you should care
Throughout your programming journey, starting here at robotics through your career in industry, you will interact with the commandline in varying ways.  For a CyberSecurity Engineer or Penetration Tester, they are trying to ethically hack into systems to ensure they are secure.  An Embedded Systems Engineer will need to communicate with microcontrollers via the commandline.   A Front-end and back-end developer will use commandline tools like Node and build tools like MAKE or GitHub Actions to build their code automatically. Lastly, if you want to have a personal server (I.E. A personal iCloud or Google Drive), most times if the User-Interface for the server goes down you will need to use the commandline to start the software/server.  Having a basic understanding of the commandline will only be a benefit to your learning!

For the following tutorial we will be using Git Bash on Windows and Terminal on Mac/Linux

## Traversing the File Tree

<!-- <Insert of File Tree at assets/images/Linux_File_Tree.png> -->
It is important to view your computer's file structure as a tree.  Where the root is the beginning of your hard drive that branches off into sub-branches containing files and other folders.  First, we will start off with just navigating this tree.  

### PWD: present working directory
The first command we will discuss is ```pwd``` which stands for present working directory.  This command will show you were your terminal currently set to.  Think of it like your File Explorer that tells you the current folder you are look at, ```pwd``` does the same thing.  It returns to you what's called a file path.

**Windows File Path**
```C:\Users\FRO\Downloads ```
**Linux/MacOS File Path**
``` /home/FRO/Downloads```

### / vs ~/
Like a tree, our file system has a root.  Actually it has two, the root and user-root.  The root is the base of the hard drive which is denoted by path ```/```.  User-root is your user folder where all information about your profile is saved.  Your Desktop, Downloads, Documents, Pictures, and Video folders live here, this path is ```C:\Users\FRO``` which also can be denoted as ```~/```.

### CD: Change Directory

### LS: List


## Creating, Viewing, & Deleting Files & Folders

### touch: Creating Files

### mkdir: Make Directories

### rm vs rm -rf


## Basic Git Commits

### git add

### git commit -m ""

### git push

### git checkout

## Advanced: Using VIM to modify files

### vim vs VS Code

## Where to go from here