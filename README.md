# ESP WiFi Communication for Arduino (Optimized)

![ESP8266/ESP32](https://img.shields.io/badge/ESP-8266%2F32-blue)
![Version](https://img.shields.io/badge/Version-1.2-green)
![License](https://img.shields.io/badge/License-MIT-orange)

Robust WiFi communication handler for ESP modules with enhanced AT command management and error handling.

## ✨ Optimized Features
- ✅ **Reliable AT Command Handling** - Full response parsing with error detection
- ✅ **Connection Verification** - Real-time WiFi and TCP status checks
- ✅ **Automatic Resource Management** - Proper connection cleanup
- ✅ **Configurable Timeouts** - Operation-specific timeout settings
- ✅ **Buffer Protection** - Prevents serial buffer overflow
- ✅ **Self-healing** - Automatic reconnection attempts

## 📦 Hardware Requirements
- Arduino board (Uno, Mega, etc.)
- ESP8266 or ESP32 module
- Sensors (for the example implementation)
  - Gas sensor (analog)
  - Temperature sensor (analog)
  - Optional third sensor

## 🔌 Wiring Guide
| ESP Module  | Arduino Connection |
|-------------|--------------------|
| TX          | RX1 (Serial1)      |
| RX          | TX1 (Serial1)      |
| GND         | GND                |
| VCC         | 3.3V*              |

*Some ESP modules require 5V - check your module specifications

## ⚙️ Configuration
```cpp
// Network credentials
const char* ssid = "YourSSID";
const char* password = "YourPassword";

// Server details
const char* server = "192.168.1.100"; // Your server IP
const int port = 80; // Your server port

// Timeout settings (ms)
const unsigned long WIFI_TIMEOUT = 30000; // 30s WiFi timeout
const unsigned long TCP_TIMEOUT = 10000;  // 10s TCP timeout

## 📜 Version History
| Version | Changes |
|---------|---------|
| 1.2 | Added connection verification, improved error handling, timeout management |
| 1.1 | Initial release with basic functionality |
