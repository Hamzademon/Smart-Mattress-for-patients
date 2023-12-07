# Smart-Mattress-for-patients
Smart Mattress for Health Monitoring & Pressure Ulcer Prevention
Overview
This repository documents the development of a smart mattress system designed to monitor health indicators and prevent pressure ulcers in individuals. The system incorporates a series of electronic components and circuits to achieve these goals.

Circuit Components
Boost & Buck Converters
Boost Converter: Raises DC voltages.
Buck Converter: Lowers DC voltages.
For the sensing circuit requiring 5V, buck converters step down 12V DC to 5V DC. Additionally, to power output channels with 70V, two boost converters are connected in series (24V input → 70V output).

Comparator & Sensors
Comparators: Regulate channel outputs based on voltage comparisons.
Sensors: Resistive elements sensitive to applied force.
The sensors' resistance changes with force application. Connected to comparators, force application triggers voltage changes, altering channel outputs. Ten comparators regulate ten channels.

Arduino Nano Control
Arduino Nano: Controls channel activation.
Pins control channel groups. Optocouplers receive signals from the Arduino to allow 70V through transistors. Frequency adjustment via analog input (A0) connected to a variable resistor.

Optocouplers & Output Control
Optocouplers: Configured in an H-bridge setup for output control.
Optocouplers enable channel outputs. Switches accompany each output for individual channel control.

Application for Health Monitoring
Pressure Ulcer Prevention
Sensor-based Control: Sensors detect force changes, altering channel outputs.
Channel Activation: High sensor resistance keeps channels off; low resistance toggles channels.
This functionality aims to prevent pressure ulcers. When no force is applied, channels remain off. Force application triggers channel activation, alleviating pressure points.

Contribution
The repository includes:

Schematics
PCB designs
3D circuit views
Conclusion
The smart mattress system utilizes electronic circuits to monitor health indicators and prevent pressure ulcers. This documentation provides a comprehensive guide for understanding and contributing to the development of this innovative solution.
