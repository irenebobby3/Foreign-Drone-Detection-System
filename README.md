# Foreign Drone Detection System

## Project Overview

The Foreign Drone Detection System is an academic mini project developed using ESP32 microcontrollers, LoRa wireless communication and an ultrasonic sensor.

The prototype demonstrates how nearby objects can be detected and how received drone identification messages can be classified as authorized or unidentified.

## Objectives

- Detect nearby objects using an ultrasonic sensor.
- Establish wireless communication using LoRa technology.
- Identify authorized and unidentified drone IDs.
- Display identification status using LED indicators.
- Monitor sensor readings and communication data through the Serial Monitor.

## Hardware Requirements

| Component | Quantity |
|---|---:|
| ESP32 Dev Module | 1 |
| ESP32-S3 | 1 |
| LoRa-02 (SX1278) | 2 |
| LoRa Antenna | 2 |
| HC-SR04 Ultrasonic Sensor | 1 |
| Green LED | 1 |
| Yellow LED | 1 |
| Red LED | 1 |
| Push Button | 1 |
| Resistors | As required |
| Jumper Wires | As required |
| Breadboard | 1 or more |

## Working Principle

The system consists of two main units:

**1. Drone-Side Unit**
- Uses ESP32-S3 and LoRa-02.
- Transmits a unique identification message wirelessly.

**2. Ground Station**
- Uses ESP32, LoRa-02 and HC-SR04.
- Detects nearby objects within a predefined 2-metre range.
- Receives identification messages through LoRa.
- Compares the received ID with the predefined authorized ID.

## LED Status Indication

| LED | Indication |
|---|---|
| Green | Authorized drone |
| Yellow | Object detected, identification pending |
| Red | Foreign or unidentified ID |

## Software Requirements

- Arduino IDE 2.x
- ESP32 Board Package
- Arduino LoRa Library
- Arduino C/C++
- SPI Library
- Serial Monitor

## Project Architecture

Drone-Side Unit → LoRa Communication → Ground Station → Identification Verification → LED Status Indication

## Applications and Learning Outcomes

- Embedded system development
- Wireless communication using LoRa
- ESP32 programming and interfacing
- Ultrasonic sensor interfacing
- Digital status indication
- Microcontroller-based system integration

## Project Type

Academic Group Mini Project – Electronics and Communication Engineering

**Note:** This is an educational prototype. Object detection and ID matching do not constitute secure drone authentication or a validated drone detection system.
## Project Gallery

### Drone
![Drone](images/Drone.png)

### Ground Side Drone
![Ground Side Drone](images/GroundSideDrone.png)
