# Arduino Ultrasonic Sensor + Servo Motor

A simple Arduino project using an **HC-SR04 ultrasonic sensor** to detect nearby objects and control an **SG90 servo motor**.

## Project Overview

- Object at **10 cm or closer** → servo moves to **90°**
- Object farther than **10 cm** → servo returns to **0°**
- Distance is displayed in the Arduino Serial Monitor.

![Project Setup](images/project.jpg)

## Components

- Arduino UNO
- HC-SR04 Ultrasonic Sensor
- SG90 Servo Motor
- Breadboard
- Jumper wires
- USB cable

## Circuit Connections

### HC-SR04 → Arduino UNO

| HC-SR04 | Arduino UNO |
|---|---|
| VCC | 5V |
| GND | GND |
| TRIG | D9 |
| ECHO | D8 |

### SG90 Servo → Arduino UNO

| Servo Wire | Arduino UNO |
|---|---|
| Red | 5V |
| Brown/Black | GND |
| Yellow/Orange | D7 |

## How It Works

1. Arduino sends a trigger pulse to the HC-SR04.
2. The sensor measures the returning ultrasonic echo.
3. Arduino calculates the distance in centimeters.
4. If the distance is **≤ 10 cm**, the servo moves to **90°**.
5. If the distance is **> 10 cm**, the servo returns to **0°**.
6. The distance is printed to the Serial Monitor at 9600 baud.


## Demo

🎥 **YouTube Demo:**  
https://www.youtube.com/watch?v=u6cNqhZgPTE

## Experiment

The activation distance and servo angle can be changed to test different behaviors, such as 15 cm, 45°, or 180°.

## Learning Outcome

This project demonstrates basic Arduino digital I/O, ultrasonic distance measurement, conditional logic, and servo motor control.
