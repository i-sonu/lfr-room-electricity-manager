# lfr-room-electricity-manager
A scalable, non-invasive robot system that autonomously patrols building corridors, detects room occupancy via multi-sensor fusion, and controls electrical loads through wireless switching — no rewiring required.

<img width="1280" height="1018" alt="image" src="https://github.com/user-attachments/assets/02872ed1-7a8b-4c95-a7aa-6a0527894986" />

Components needed:
**LFR ESP32:**
ESP32 dev board
L298N motor driver
2x DC motors
8x IR sensors
PIR sensor
Sound sensor module

**Receiver ESP32:**
ESP32 dev board
LED
220Ω resistor
Push button

**Common:**
Jumper wires
Power supply / LiPo battery


**LFR CONNECTIONS:**
 ___________________________________________________
| Pin           | Connected To                      |
|---------------|-----------------------------------|
| GPIO 4        | PIR sensor OUT                    |
| GPIO 15       | Sound sensor OUT                  |
| GPIO 18 (ENA) | L298N ENA (PWM for left motor)    |
| GPIO 5 (IN1)  | L298N IN1                         |
| GPIO 19 (IN2) | L298N IN2                         |
| GPIO 23 (ENB) | L298N ENB (PWM for right motor)   |
| GPIO 21 (IN3) | L298N IN3                         |
| GPIO 22 (IN4) | L298N IN4                         |
| GPIO 32       | IR Sensor 1 (leftmost)            |
| GPIO 33       | IR Sensor 2                       |
| GPIO 25       | IR Sensor 3                       |
| GPIO 26       | IR Sensor 4                       |
| GPIO 27       | IR Sensor 5                       |
| GPIO 14       | IR Sensor 6                       |
| GPIO 12       | IR Sensor 7                       |
| GPIO 13       | IR Sensor 8 (rightmost)           |
| 3.3V / 5V     | VCC of all sensors                |
| GND           | Common GND                        |
|___________________________________________________|

**RECIEVER CONNECTIONS:**
 ________________________________________________________
| Pin     | Connected To                                 |
|---------|----------------------------------------------|
| GPIO 2  | LED (~220Ω resistor to GND)                  |
| GPIO 4  | Push button (other leg to GND, INPUT_PULLUP) |
| GND     | Common GND                                   |
|________________________________________________________|
