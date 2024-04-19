# Bluetooth Controlled RC Car

This repository contains the Arduino code for a Bluetooth-controlled RC car using the Adafruit Motor Shield. The code allows the user to control the car's movements (forward, backward, left, and right) using Bluetooth commands sent from a smartphone or other Bluetooth-enabled devices.

## Table of Contents

- [Requirements](#requirements)
- [Setup](#setup)
- [Usage](#usage)
- [Troubleshooting](#troubleshooting)

## Requirements

- Arduino board (e.g., Arduino Uno)
- Adafruit Motor Shield
- DC motors (4 in total)
- HC-05 Bluetooth module
- SoftwareSerial library (for Bluetooth communication)
- AFMotor library (for motor control)
- Power source for the motors (e.g., battery pack)
- Power source for the Arduino board (if separate from the motor power source)

Before uploading the code to your Arduino, ensure you have the AFMotor library installed. You can install it using the Library Manager in the Arduino IDE.

## Setup

1. **Hardware Setup**:
    - Connect the Adafruit Motor Shield to your Arduino board.
    - Connect the DC motors to the appropriate motor ports on the Motor Shield.
    - Connect the HC-05 Bluetooth module to the Arduino:
        - RX pin of the HC-05 to pin 9 on Arduino.
        - TX pin of the HC-05 to pin 10 on Arduino.
    - Connect the appropriate power sources to the Arduino and Motor Shield.
    - Ensure the jumper on the Motor Shield is set correctly to enable or disable the motors as needed.

2. **Code Setup**:
    - Clone this repository to your local machine.
    - Open the Arduino IDE and load the `.ino` file from this repository.
    - Choose the correct board and port in the Arduino IDE.
    - Upload the code to your Arduino board.

3. **Bluetooth Pairing**:
    - Pair your Bluetooth-enabled device (e.g., smartphone) with the HC-05 Bluetooth module.
    - The default pairing code for the HC-05 is typically `1234` or `0000`.

## Usage

- After setting up and uploading the code, you can control the car using a Bluetooth terminal app on your smartphone.
- The app should be connected to the HC-05 module, and you can send the following commands to control the car:

  - `'F'`: Move the car forward.
  - `'B'`: Move the car backward.
  - `'L'`: Turn the car left.
  - `'R'`: Turn the car right.

## Troubleshooting

- **Communication Issues**: Ensure the correct RX and TX pins are connected between the HC-05 and the Arduino. Also, verify the baud rate is set correctly in both the code and the Bluetooth terminal app.
- **Motor Issues**: Double-check the connections between the motors and the Motor Shield. Also, verify that the power source for the motors is sufficient and properly connected.


This project is released under the [MIT License](LICENSE).

--- 

The README file is straightforward and covers all necessary aspects of the project. Make sure the project file and the `LICENSE` file are included in your repository if you have a specific license. Let me know if you need any other improvements.
