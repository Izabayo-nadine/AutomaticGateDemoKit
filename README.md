🚦 Automatic Gate Control System with Ultrasonic Sensor and Servo
This Arduino project implements an automatic gate control system using an ultrasonic sensor, servo motor, LEDs, and a buzzer. It simulates a basic security or convenience system where a gate automatically opens when an object (e.g. a person or vehicle) is detected within a certain distance.

📌 Features
Distance Detection: Uses an ultrasonic sensor to measure proximity.

Automatic Gate Operation:

Opens when an object is detected within 20 cm.

Closes 5 seconds after the object leaves the range.

Visual & Audio Indicators:

Red LED ON: Gate is closed.

Blue LED ON: Gate is open.

Buzzer beeps for 5 seconds while the gate is open.

Smooth Servo Movement: Prevents servo motor from jerky transitions.

🔧 Hardware Requirements
Ultrasonic Sensor (HC-SR04)

Servo Motor (e.g. SG90)

Red LED

Blue LED

Buzzer

Arduino Uno (or compatible)

Resistors (for LEDs)

Breadboard & Jumper Wires

🧠 How It Works
The ultrasonic sensor continuously measures the distance ahead.

If an object is detected within 20 cm, the servo opens the gate and activates the blue LED and buzzer.

If no object is detected for 5 seconds, the servo closes the gate, reactivates the red LED, and turns off indicators.

🗂️ Pin Configuration
Component       	            Pin
Ultrasonic TRIG             	D2
Ultrasonic ECHO	              D3
Red LED	                      D4
Blue LED	                    D5
Servo Motor	                  D6
Buzzer	                      D12
GND (dummy pins)	            D7, D8 (set LOW)
