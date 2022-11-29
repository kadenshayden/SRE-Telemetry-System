# SRE-Telemetry-System

The intended goal of this project is to make viewing of CAN bus data easy and accessible for 
Spartan Racing (SR/SRE) FSAE cars. CAN bus data includes tire temp, battery temp (for EV's),
motor temp, oil Pressure, and any other information communiate through the protocol. 

Current state of Telemetry:
CAN bus information must be transferred over physical connection to a laptop. This means 
the data must be copied while the car is stationary. 

As an initial prototype of the project to test feasibility, two RF69 packet radios were programmed. 
One is a dedicated server while the other is a client, both hooked up to seperate Arduino Mega's.
Test code is provided by the Radiohead library. 

![alt text](https://github.com/kadenshayden/SRE-Telemetry-System/blob/main/simpleVCU%20senderreceiver%20prototype%20node.png?raw=true)

The obvious worry is that Arduino hardware isn't weatherproofed or vibration isolated. An easy fix for this is to enclose it in an aluminum casing, utilinzg rubber standoffs from McMaster to isolate the board from vibration. I haven't heard of anybody having a board die from vibration, but you wouldn't want it to happen on the track. 

Goal:
A long term goal of the project is to use off-the-shelf hardware to communicate data with the 
host laptop in real time. So while the car is running around the track, the team can monitor 
data and make sure that nothing abnormal is happening. 

Using KX Dashboards, Arduino UNO's, and long range packet radios we will be able to graph and organize data in real time. 

Team:
Kaden Golda
Ian Hunter
