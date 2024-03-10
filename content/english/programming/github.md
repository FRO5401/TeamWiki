---
title: "Github 101"
meta_title: ""
description: ""
image: "/images/gifty-gour01.PNG"
categories: ["Programming"]
#author: "Muffin Man"
# tags: ["nextjs", "tailwind"]
draft: false
---

**Intro to Terminal**\
The terminal is what you think of when watching a programmer in a movie. There is no clickable user interface with a mouse, everything happens from your keyboard. There are two main types of terminals with syntactical differences but they generally can perform the same actions. Bash is the terminal on Linux or MacOS devices whereas CMD runs on Windows. The benefit of using the command line is that your fingers stay on the keyboard & nearly anything you can do with the mouse can be done in less time the command line.\
While you’re here at robotics you mostly will be using CMD, unless you choose to learn Linux (which I recommend to the upperclassman). For the command line, you will use it mostly for copying files, creating folders, & git.\
‘What is git?’ you might be asking, it is a software version control protocol that allows multiple users/machines to work on a codebase at a time. Git allows users to pull, push, merge, & revert code from a server. Here we will discuss how to perform basic git commands, there are more complicated commands but we just need you to know these basics.

For a full tutorial of git please use the following resources:

- https://ohmygit.org/
- https://www.w3schools.com/git/
- Team Presentation: https://docs.google.com/presentation/d/1j5qtgoRv2GGTz7wum2VJOVj4y_qC2zrYVYq54Ko1uc8/edit?usp=sharing

**Initialize a new Repo**\
You probably will not need to do this often for robotics but if you ever need to start a new project you’d like in git do the following.
```
git init
git commit -m “initial commit” 
```
**Clone Repo**\
Cloning a repo means, as the name suggests, get a local copy of a repository that is in git. You can do this to brand new repository or an established one. Here Is an example to clone the 2023 First Powerup Repo.

1. Go to GitHub.com
2. Click your user icon & select Your Organizations
3. Select Team5401
4. Find the repo you’d like to clone, in our case ChargedUp2023 & select it
5. Select the big green Code button, then make sure that the HTTPS button is selected, & finally, click the copy button next to url
6. Open your terminal, can cd to the folder you want to clone the repo to. For example, if I wanted to cd to the Documents folder. If you want to go to a folder inside of the documents called Programming, use the second command.
```
cd Documents
Or
cd Documents \ Programming 
```
7. Lastly, run the following command, but instead of pasting in "\<link to repo\>," paste the link you copied from GitHub.
```
git clone <link to repo> 
```

**Committing Code**\
Committing means taking code that you have written & sending them to the parent repository. Commits can be small, like fixing a typo in a comment, or large, such as an entire sub-system for the robot (not preferred). A question you may be asking is, “When should I commit?”, and that is a tricky question.

There is no standard answer but there is a motto that says to commit “early & often”. The idea is that the more commits there are, the more points there are to revert to in the future. Imagine you commit code that breaks the robot, if you commit very infrequently when you have to revert a lot of code will change even if there is a tiny bug. In general, every time you have a new working aspect of your code, it should be committed. For example, if you are coding the drive base for autonomous here are suggested commit points
- Creating the new Java file with boilerplate
- Accessing drive-base & sensor classes
- Calling the autonomous from main code
```
git commit -m “<some message here>” 
```
Your commit messages should be specific to what was done & be a sentence @ max & minimum. Examples messages:
- “Created new autonomous file”
- “Meshing sensor & drivebase data”
- “Finalized autonomous & called it from main”

**Pushing / Pulling code**\
Pushing code means taking committed code from your local machine to the remote branch. Pulling code does the opposite, it takes code that is in the remote branch to your master branch. If your code locally doesn’t match up with the remote branch there may be merge conflicts that require a rebase. If so, seek out the programming lead or mentor.
```
git pull 
git push 
```

**Creating / Checking out Branch**\
A branch is the separate progression of code away from the main branch. Branches allow you to work on a new feature & test it with the full code base while it’s still in development. When you’re done with the feature, you will need to make a Pull Request to merge your branch into the master branch. To create a new branch off of master do the following:
```
cd <file path to repo>
git checkout master
git pull
git checkout -b ‘<name of new branch> 
```

**Pull requests**\
When your feature is done & ready to be tested & merged, a Pull Request needs to be created from GitHub.
1. Navigate to the GitHub repo, such as Crescendo2024
2. Select Pull Request & New Pull Request
3. Select the compare dropdown & find the name of your branch
4. Select Create Pull Request
5. Fill in the title of the PR as the name of the issue you are working on. Inside GitHub Projects, there should be a name for your issue, place that name where it says ‘Swerve drive base in this photo. For the description, use a bulleted list to describe snippets of everything your PR does.
6. Open a Pull Request Screen