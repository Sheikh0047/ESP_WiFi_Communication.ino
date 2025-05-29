# ESP WiFi Communication for Arduino

This project handles WiFi connection and data transmission using an ESP module (ESP8266/ESP32) with Arduino.

## Features
- WiFi connection management
- HTTP GET requests to send sensor data
- Timeout handling for robust communication
- Debugging output via Serial Monitor

## Hardware Requirements
- Arduino board
- ESP8266 or ESP32 module
- Sensors (optional for the example)

## Setup
1. Update `ssid` and `password` in the sketch
2. Set your server IP and port
3. Connect ESP module to Arduino's Serial1

## Wiring
- ESP TX -> Arduino RX1
- ESP RX -> Arduino TX1
- ESP GND -> Arduino GND
- ESP VCC -> 3.3V (check your module requirements)
