<meta name="author" content="Mahdi Zeinali">
<meta name="account" content="mahdizynali">
<meta name="description" content="mahdi Zeinali github account">
<meta name="copyright" content="mahdi zeinali 2023">
<meta name="keywords" content="mahdi zeinali, mahdizynali, mrl-hsl, mrl, hsl, zeinali, mahdi zynali">

<b><h2 align="center">.:: Soccer-Robot-Playground ::.</h4></b>

<p align="center">
<a href="https://github.com/mahdizynali/Soccer-Robot-Playground"><img src="https://img.shields.io/badge/Version-1.2.1-brightgreen" alt="HSL" width="100"></a>
<a href="https://github.com/mahdizynali/Soccer-Robot-Playground"><img src="https://img.shields.io/badge/Platform-linux--64-blue" alt="HSL" width="130"></a>
<a href="https://github.com/mahdizynali/Soccer-Robot-Playground/blob/main/LICENSE.md"><img src="https://img.shields.io/badge/LICENSE-GNU-red" alt="HSL" width="110"></a>
<a href="https://github.com/mahdizynali/Soccer-Robot-Playground/network/members"><img src="https://img.shields.io/badge/Developers-2-lightgrey" alt="HSL" width="100"></a>
</p>

![alt text](https://raw.githubusercontent.com/mahdizynali/Soccer-Robot-Playground/main/images/sample.jpg)

# Table Switch

- [Introduction](#introduction)
- [Primary Dependencies](#dependencies)
- [Program Headers](#program-headers)
- [How To Run](#how-to-run)
- [Developers](#developers)
  
# Introduction

  Soccer Robot Playground is a simulation of world model which includes two section of grounds.
  
  - Real World : 
    - In this scope , program display the soccer field with an agent (a robot sample) inside it.\
    Field's coordinate is based on RoboCup soccer humanoid league laws 2022 and the agent is surrounded by a border that consist the absolute 
    playground area.\
    The features of the Real World are Movement by keyboard , Transition by mouse and a Helpwindow for declaring the keys 
    and represent the robot exact location on screen.
      
  - Model World :
    - Robot modeling is a part of program which make a simple shape of an agent and switch the location of shape into the original one.\
    To comprehend that what does modeling exactly do , consider the airplane's radar so that the radar make a shape of airplane on 
    it's screen nearby the own system.\
    But the impotant note is that the modeling system will upgrade only by agent's location in every frames !!
    
  To get more information and explanation about the World Model , refer to the [Document](https://github.com/maze80/Soccer-Robot-Playground/blob/main/Document/) of project.
  


# Dependencies
The operation system is linux-64 bit and developed on [Ubuntu 22](https://ubuntu.com/) core.\
This project is completely based on [C++ language](https://cplusplus.com/) and we have hardly tried to write the codes with simple syntax to make it
easier for understanding and help beginners to develop it much better.\
Most part of the program is powered by OpenCV version 4 in C++ form. To make it install , you can use 
this [orientation](https://dev.to/swervin/how-to-install-opencv-4-2-0-on-ubuntu-18-04-3i7l).
  
    
# Program Headers

All of the headers have connection with each other like a chain and call the other one.\
Main.cpp , make an object of world with endless circulation.

  - Config.hpp
    - It includes all libraries & workspaces & all of global variables that be used in other headers.
  - Field.hpp
    - This header contain field's class code to draw the borders which scope declaration is inside Field.cpp.
  - Robot.hpp
    - Original agent class with velocity and movement function are in this header.
  - Model.hpp
    - This header is derivated from Robot.hpp but with less options and variables.
  - World.hpp
    - Actually it's the main file of program that include drawing matrix and functions and MouseCallBack section ...
  - HelpWindow.hpp
    - class of displaying notes and status of agent.
    
    
# How To Run

At first let's download the project from Github :
```
$ sudo git clone https://github.com/mrl-hsl/Soccer-Robot-Playground.git
```

There is a CMakeLists inside the repo ; which will be used for compiling all of headers together.\
In order to build the program just open the terminal in the exact directory and then :
```
& mkdir build && cd build
```
After that try to make headers :
```
$ cmake .. && make
```
with compiling the program you try to run "soccer-main"\
And if you decide to remove the compiled files :
```
& make clean
```

# Developers

<p align="center">

<a href="https://github.com/mahdizynali"><img src="https://avatars.githubusercontent.com/u/104717705?s=120&v=4" width="100;" alt="Mahdi Zeinali"/><br /><sub><b>.:: Mahdi Zeinali ::.</b></sub></a>

<a href="https://github.com/RamtinKosari"><img src="https://avatars.githubusercontent.com/u/106661724?s=120&v=4" width="100;" alt="Ramtin Kosari"/><br /><sub><b>.:: Ramtin Kosari ::.</b></sub></a>

</p>

