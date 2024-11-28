# Siderum-Nexus #
Automation for German Equatorial Mount


## Overview

This is an initiative to automate small equatorial germanic mounts.
In its development, we used parts that are widely available practically anywhere in the world and have a low cost.


## How Does It Work?

An app calculate celestial body actual position in terms of Right Ascension and Declination.
Then, the steppers move GEM axis to the desired position and continue to track the sideral movement.


## Software

A Delphi based app make all calculations and determine the actual Right Ascension and Declination coordinates. It has a bluetooth connection with the microcontroller in the electronic circuit that controls the steppers and send this coordinate information.
The microcontroller has a C++ firmware that receives the coordinates and calculate how many turns (micro steps) each stepper in each axis to achieve the correct position.
All calculations were made taking account the necessary precision, or better if the processing "cost" is the same or almost the same.

## Hardware

Basically, in this project are used 3D printer parts like steppers, stepper drives, ESP32 microcontroller and a circuit board.



## [Electronics](https://github.com/amjorge1972/Siderum-Nexus/tree/main/electronics)
