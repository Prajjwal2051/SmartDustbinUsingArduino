# Smart Dustbin Using Arduino

A smart, contactless dustbin that automatically opens its lid when it detects someone nearby, making waste disposal more hygienic and convenient.

## Overview

This project implements a **Smart Dustbin** using Arduino, an ultrasonic sensor, and a servo motor. The dustbin detects the presence of a hand or object near its lid and opens automatically, closing after a short delay. This system promotes hygiene by reducing the need for physical contact with the dustbin lid[4][5][2].

## Features

- **Automatic Lid Opening:** Uses an ultrasonic sensor to detect objects within a preset range and triggers the lid to open via a servo motor.
- **Hands-Free Operation:** Enhances hygiene and convenience by eliminating the need to touch the dustbin.
- **Easy to Build:** Uses readily available components and straightforward Arduino code.
- **Customizable:** Detection range and lid open duration can be adjusted in the code[5].
- 
## Components Used

- **Arduino Uno (or compatible)**
- **Ultrasonic Sensor (HC-SR04)**
- **Servo Motor (SG90 or similar)**
- **Jumper Wires**
- **9V Battery or suitable power supply**
- **Dustbin with attached lid**
- **Miscellaneous:** Cardboard, tape/glue for mounting components[4][5].

## How It Works

1. **Detection:** The ultrasonic sensor continuously measures the distance to any object in front of the dustbin.
2. **Trigger:** When an object (e.g., a hand) is detected within a certain range (e.g., 2–30 cm), the Arduino receives the signal.
3. **Action:** The Arduino commands the servo motor to open the dustbin lid.
4. **Auto-Close:** After a short delay (e.g., 3 seconds), the lid closes automatically[4][5].

## Circuit Diagram

- **Ultrasonic Sensor:**  
  - VCC → 5V on Arduino  
  - GND → GND on Arduino  
  - Trig → Digital Pin (e.g., 5)  
  - Echo → Digital Pin (e.g., 6)
- **Servo Motor:**  
  - Signal → Digital Pin (e.g., 7)  
  - VCC → 3.3V or 5V  
  - GND → GND
- **Power:**  
  - 9V battery connected to Vin and GND on Arduino[5].

## Getting Started

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Prajjwal2051/SmartDustbinUsingArduino.git
   ```
2. **Assemble the Hardware:**  
   Connect the ultrasonic sensor and servo motor to the Arduino as per the circuit diagram.
3. **Upload the Code:**  
   Open the Arduino IDE, load the provided code, and upload it to your Arduino board.
4. **Power Up:**  
   Attach the battery or connect via USB. Test the system by moving your hand near the sensor.

## Customization

- **Detection Range:**  
  Adjust the threshold distance in the code to change how close an object must be to trigger the lid.
- **Lid Open Time:**  
  Modify the delay in the code to keep the lid open for a longer or shorter duration[5].

## Benefits

- **Improved Hygiene:** No need to touch the lid, reducing the spread of germs[4].
- **Convenience:** Effortless waste disposal.
- **Educational:** Great project for learning about sensors, Arduino programming, and automation.
