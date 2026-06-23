# Voice Controlled Room Lighting

![SURGE](https://img.shields.io/badge/SURGE099-Research_Project-red)
![ESP32](https://img.shields.io/badge/ESP32-IoT-blue)
![Wit.ai](https://img.shields.io/badge/Wit.ai-NLP-green)
![Arduino](https://img.shields.io/badge/Arduino-C%2B%2B-orange)
![IIT Delhi](https://img.shields.io/badge/IIT%20Delhi-EE-maroon)


A smart home lighting system that enables voice-based appliance control using ESP32, INMP441 microphone and Wit.ai.

---

## Overview

This project aims to build an Alexa-like voice assistant for controlling room lighting.

The system captures voice commands using an INMP441 digital microphone connected to an ESP32. Audio is transmitted over WiFi to Wit.ai for speech recognition and intent extraction. Based on the recognized command, the ESP32 controls a relay module to switch the room light ON or OFF.

---

## Features

- Voice controlled light ON/OFF
- ESP32 based IoT architecture
- WiFi communication
- Cloud NLP using Wit.ai
- Low power embedded implementation

---

## System Architecture

```text
User Voice
    ↓
INMP441 Microphone
    ↓
ESP32
    ↓ WiFi
Wit.ai API
    ↓ Intent
ESP32
    ↓
Relay Module
    ↓
Room Lighting
```

---

## Hardware Used

| Component | Purpose |
|----------|---------|
| ESP32 | Main controller |
| INMP441 | Digital microphone |
| Relay Module | AC load switching |
| Wit.ai | Speech recognition |

---

## Platform Evaluation

The following platforms were evaluated:

| Criteria | ESP32 | Raspberry Pi |
|---------|------|--------------|
| Power Consumption | Low | High |
| WiFi/Bluetooth | Built-in | Built-in |
| Boot Time | < 1 sec | ~30 sec |
| Cost | Low | Moderate |

**ESP32 was selected due to its low power consumption and suitability for embedded IoT applications.**

---

## Progress Report

Detailed progress report available here:

📄 [SURGE099 Progress Report](docs/SURGE099_Progress_Report.pdf)

---

## Future Work

- Implement I2S audio capture firmware
- Improve noise robustness
- Add local TinyML keyword spotting
- Support multiple appliances
- Optimize latency

---

## Author

**Abhishek Mehta**

B.Tech Electrical Engineering  
IIT Delhi
