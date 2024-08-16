---
layout: page
title: Arduino Language Support
description: Extension for VS Code
img: assets/img/als/icon.jpeg
importance: 1
category: work
related_publications: false
---

# Purpose

I am a robotics enthusiast and, on one certain occasion, wanted to edit my Arduino project in Visual Studio Code.

However the following issues arose which convinced me to make my own extension for it.

- When using C++ as the language mode for using .ino files, it doesn't recognize any of the arduino specific functions and treats them as an error.
- Microsoft's extension for arduino only has "arduino output" as an option for language mode.

<br>
<br>

Using "C++" as language mode for .ino files

![.ino with C++](assets/img/als/Screenshot(7).png)

## What's wrong with Microsoft's Arduino extension?

By default, "arduino output" doesn't use Syntax Highlighting which makes it difficult to edit/create programs as it becomes confusing to navigate through it, and monotonous enough to make a person quit.

<br>
<br>

Using "arduino-output" as language mode for .ino files

![.ino with arduino-output](assets/img/als/Screenshot(8).png)

## What of the other extensions?

There was one certain extension that I took a liking to but the themes that came along with it didn't match the original themes of the Arduino IDE, though it is somewhat similar.

---

# Goal

In this extension I am doing the following at the moment:

- Include Syntax Highlighting
- Add Arduino as default language for .ino files, this will disable C++ linter automatically each time you open .ino file allowing you to avoid the numerous errors formed due to arduino-specific functions
- Include 2 Themes as a bonus for users who prefer the Arduino IDE's charming looks
    - Arduino IDE Light
    - Arduino IDE Dark

<br>
<br>

I am also thinking about adding my own linter but that is something I won't be doing for quite a while.
---

# Exapmle

## Themes
### Arduino IDE Light
![Homepage](assets/img/als/Screenshot(4).png)
![Editor](assets/img/als/Screenshot(2).png)
### Arduino IDE Dark
![Homepage](assets/img/als/Screenshot(5).png)
![Editor](assets/img/als/Screenshot(1).png)

---

## Configure Language
If not set by default, click on the language mode button in the status bar.<br> It is most likely in the bottom right, with either "C++" or "Plain Text" written on it.
That will open this menu:<br>
![Language Mode Menu](assets/img/als/Screenshot(6).png)<br>
Click on Arduino to use it or, click on "Configure File Association for '.ino'" and then click on Arduino to set it up permanently

---

# CHANGELOG

All notable changes to the "Arduino Language Support" extension will be documented in this file.

## Unreleased
- v2.0.0
  - Added
    - .ino file linter

## Released
- v1.0.4
  - Fixed
    - Allowed to be used by older versions of VS Code upto and including 1.43.0
- v1.0.3
  - Fixed
    - Screenshot display issue
- v1.0.2
  - Modified
    - License : Adopted Apache-2.0
    - README.md : Fixed Typos
- v1.0.1
  - Modified
    - Icon.jpg : Changed icon
- v1.0.0
  - Added
    - Arduino IDE Light theme
    - Arduino IDE Dark theme
    - .ino Grammar file