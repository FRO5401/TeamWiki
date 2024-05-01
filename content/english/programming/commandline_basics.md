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
The first command we will discuss is ``pwd`` which stands for present working directory.  This command will show you were your terminal currently set to.  Think of it like your File Explorer that tells you the current folder you are look at, ``pwd`` does the same thing.  It returns to you what's called a file path.

**Windows File Path**
``C:\Users\FRO\Downloads ``
**Linux/MacOS File Path**
`` /home/FRO/Downloads``

### / vs ~/
Like a tree, our file system has a root.  Actually it has two, the root and user-root.  The root is the base of the hard drive which is denoted by path ``/``.  User-root is your user folder where all information about your profile is saved.  Your Desktop, Downloads, Documents, Pictures, and Video folders live here, this path is ``C:\Users\FRO`` which also can be denoted as ``~/``.

### CD: Change Directory
To traverse the file tree we need to change directories both up and down the document tree.  The cd command does just this, to use it you just need to provide 1 parameter, where you want to go.  For example, from the user root directory (``~/`` or ``C:\Users\FRO``), if we want to navigate to the Desktop, we would say ``cd Desktop``.  Like many commands but especially for file paths and names, case matters!  Desktop and desktop are not the same, since the user (you) can name files anything they want.  Once we are on the desktop, ``C:\Users\FRO\Desktop`` to go back we to user-root we can either say ``cd ~/`` or ``cd ..\`` both do the same thing in this context.  ``..\`` means to go up the parent directory from the current directory.  Desktop's parent is our user-root.  If there is a folder on the desktop called ``2023_Robot_Code`` that was at ``C:\Users\FRO\Desktop\2023_Robot_Code``, ``cd ~/`` and ``cd ..\`` would NOT do the same thing.  ``~/`` would still take you to the user-root but ``..\ `` would go up to the Desktop directory (``C:\Users\FRO\Desktop``) since it is the parent of 2023_Robot_Code.

### LS: List
When using File Explorer we will see files in a given folder, ``cd`` only takes us to the folder but does not show us what the contents are.  That is where the ``ls`` command comes in.  It will show you all files you would see File Explorer in the terminal output.  However there are 'hidden files' that are prefixed with a ``.`` in-front of their name, a common example is ``.gitignore``.  To see these files you will say ``ls -la``, this will show hidden files as well as the file/folder owner, the creation/edit date, and the file permissions.  All of which are outside the scope of this basic tutorial.

## Creating, Viewing, & Deleting Files & Folders

### touch: Creating Files
To create a file(s) simply navigate to the directory you want them to reside in and use the ```touch``` command and just pass in the name of the file you'd like to create.  For example to make a file called main.java you would say ```touch main.java```.  To create more than 1 file, just seperate the names by a space, ```mkdir main.java Constants.java Arm.java```.  <u>**It is important to add the file extension to the end of the filename so your computer knows what type of file you created**</u>

### mkdir: Make Directories
To create a directory(s) simply navigate to the directory you want them to reside in and use the ```mkdir``` command and just pass in the name of the directory you'd like to create.  For example to make a directory called 2024_Build_Season you would say ```mkdir 2024_Build_Season```.  To create more than 1 folder, just seperate the names by a space, ```mkdir 2024_Build_Season 2025_Build_Season 2026_Build_Season```.

### rm vs rm -rf
Just like how there are two different commands to create files and folders, there are two different commands to delete them.  Use ```rm``` and the name of file(s) and ```rm -rf``` and the name of directory(s) to delete their respective item.

```rm main.java Constants.java Arm.java``` to remove the example <u>files</u>

```rm -rf 2024_Build_Season 2025_Build_Season 2026_Build_Season``` to remove the example <u>directories</u>.

### cat: catenate
To view the contents of files you can say ```cat <Path to file>```.  CAT can merge multiple files into 1 and edit multiple files at once.  Again, that is out of the scope of this tutorial but feel free to research its other applications.

## Basic Git Commits

These commands are meant to replace your need for GitHub Desktop.  Hopefully you will find that this is way quicker than opening another application and clicking multiple buttons.  There are still other functions that you will need to use GitHub Desktop for, but these are your most common ones.

### git status 
This command will show you files in the repo that have been modified, added, or deleted.  Simply use ```git status``` in the the terminal.  Example output below:

```bash
    On branch Commandline-Basics
    Your branch is up to date with 'origin/Commandline-Basics'.

    Changes not staged for commit:
    (use "git add <file>..." to update what will be committed)
    (use "git restore <file>..." to discard changes in working directory)
            modified:   content/english/programming/commandline_basics.md

    no changes added to commit (use "git add" and/or "git commit -a")
```

### git add
This command will add a file or files to staged, allowing you to perform subsequent commands on those files.  Two examples are ```git add <path to a specific file>``` and ```git add .```, the first will add only 1 file where the other will add ALL files that have been changed/added/deleted

### git commit -m ""
This command commits the files that were staged with ``git add`` with a message of your choice.  For the message itself, there are multiple conventions on what to say.  One example is called [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/#summary) and other is just adding a single sentence of what you did.  Example command would be ```git commit -m "feat: added commandline basics page"```

### git push
This command _pushes_ commits or branches from your local machine to your remote branch(GitHub).  For pushing commits you can just say ```git push```.   For pushing a _**new**_ branch for the **FIRST** time, you can use ```git push --set-upstream origin <Name of Branch>```.

### git checkout
Checkout allows you to change and create branches.  To switch to the ```main``` branch from any other, you can say ```git checkout main```.  To create a new branch based on the current one your on, which you can get from [git status](#git-status), you will say ```git checkout -b "<Name of NEW branch>"```

## Advanced: Using VIM to modify files
VIM stands for "**V**isual **I**nstrument i**M**proved" which is a way to edit files from the terminal.  If you need to edit a single file, you can do you pretty easily with VIM.  It is recommended for you guys just getting started to use VS Code to edit multiple files.  It is encourage for you to experiment using VIM and get familiar with it.  There are other terminal editors such as nano and vi but Jimmy's personal recommendation is vim.

Here are some links to edit files:
* [VIM Tutorial - (Text)](https://www.freecodecamp.org/news/vim-beginners-guide/)
* [VIM Tutorial - (Video)](https://www.youtube.com/watch?v=-txKSRn0qeA)
* [Nano Tutorial - (Text)](https://linuxhandbook.com/nano-editor-basics/)
* [Nano Tutorial - (Video)](https://www.youtube.com/watch?v=gyKiDczLIZ4)
* [VI Tutorial - (Text)](https://www.thegeekdiary.com/basic-vi-commands-cheat-sheet/)
* [VI Tutorial - (Video)](https://www.youtube.com/watch?v=-_DvfdgR-LA)

## Where to go from here

* Git Rebase / Reset
* Chmod
* bash scripting
* PowerShell
