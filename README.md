# Smart Dustbin with Arduino and Ultrasonic Sensor

Welcome to the Smart Dustbin project! This project demonstrates how to build a smart dustbin using an Arduino Uno, an ultrasonic sensor, and a micro servo motor. The dustbin opens its lid automatically when it detects an object nearby, using ultrasonic sensor technology, and then closes after a set period.

## Table of Contents
- [Introduction]
- [Hardware Components]
- [Software Required]
- [Circuit Diagram]
- [Working Concept]
- [Installation and Setup]
- [Usage]

## Introduction
In the era of contactless technology, the Smart Dustbin aims to reduce touchpoints and improve hygiene. This dustbin uses an ultrasonic sensor to detect when someone approaches, signaling the Arduino to open the lid. After a brief delay, the servo motor closes the lid automatically.

## Hardware Components
- Arduino Uno
- Ultrasonic Sensor HC-SR04
- SG90 Micro Servo Motor
- 9V Battery
- Power Supply
- Dustbin (for the lid mechanism)

## Software Required
- Arduino IDE (for programming the Arduino)

## Circuit Diagram
Circuit diagram is given in the assets folder

Connection Procedure :

- The ultrasonic sensor's `echo` and `trig` pins connect to Arduino Uno's pins 5 and 6, respectively.
- The sensor's `VCC` connects to Arduino's 5V, and its `GND` connects to Arduino's `GND`.
- The servo motor's signal pin connects to pin 7 on Arduino, while `GND` and positive connect to Arduino's `GND` and 3.3V, respectively.
- A 9V battery connects to the Arduino's `Vin` pin for power.

## Working Concept
The ultrasonic sensor detects objects in front of the dustbin. The Arduino receives this signal and instructs the servo motor to open the lid. After a delay (e.g., 3 seconds), the servo motor closes the lid. This system reduces the need for physical contact when disposing of trash.

## Installation and Setup
1. Install the Arduino IDE on your computer.
2. Connect the Arduino Uno to your computer via a USB cable.
3. Open the Arduino IDE and upload the provided code to the Arduino.
4. Assemble the hardware components according to the circuit diagram.

## Usage
After assembling the components and uploading the code, power the Arduino with the 9V battery. Approach the dustbin, and the ultrasonic sensor will trigger the servo motor to open the lid. After 3 seconds, the lid will close automatically.
