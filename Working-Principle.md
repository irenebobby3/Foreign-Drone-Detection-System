# Working Principle – Foreign Drone Detection System

## 1. Introduction
The Foreign Drone Detection System consists of two main units: a drone-side unit and a ground station. Both units communicate using LoRa wireless technology.

## 2. Drone-Side Operation
- The ESP32-S3 acts as the controller.
- The LoRa-02 module transmits the drone identification message.
- Each identification message represents an authorized or unidentified drone for demonstration purposes.

## 3. Ground-Station Operation
- The HC-SR04 ultrasonic sensor continuously measures the distance to nearby objects.
- When an object enters the predefined 2-metre range, the ground station starts the identification process.
- The LoRa-02 module receives the identification message.
- The ESP32 compares the received ID with the predefined authorized ID.

## 4. Identification and Indication

| LED | Status |
|---|---|
| Green | Authorized ID matched |
| Yellow | Identification pending |
| Red | Unidentified ID |

## 5. Communication
LoRa communication is used to exchange identification messages between the drone-side unit and the ground station. The received data is processed by the ESP32.

## 6. Conclusion
The prototype demonstrates the integration of ultrasonic sensing, wireless communication, microcontroller programming and LED-based status indication.

**Note:** This is an educational prototype. It does not provide secure drone authentication or independently confirm that a detected object is a drone.
