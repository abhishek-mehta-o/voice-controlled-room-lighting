<div align="center">

# Voice Controlled Room Lighting

### SURGE099 Research Project  
### Alexa Equivalent for Smart Home Control

**Abhishek Mehta**  
B.Tech Electrical Engineering, IIT Delhi  
Roll No: 2024EE30767

![SURGE](https://img.shields.io/badge/SURGE099-Research_Project-red)
![ESP32](https://img.shields.io/badge/ESP32-IoT-blue)
![Wit.ai](https://img.shields.io/badge/Wit.ai-NLP-green)
![Arduino](https://img.shields.io/badge/Arduino-C++-orange)
![Status](https://img.shields.io/badge/Status-In_Progress-yellow)

</div>

---

## Overview

This project aims to develop a voice-controlled smart lighting system that functions as a lightweight **Alexa-equivalent** for home automation.

The system captures voice commands using an **INMP441 digital microphone** connected to an **ESP32**, transmits audio over Wi-Fi, performs speech recognition using **Wit.ai**, and controls room lighting via a relay module.

The objective is to create an efficient, low-cost, and scalable embedded solution for voice-based smart home control.

---

# Features

- Voice-controlled ON/OFF switching
- Wi-Fi enabled communication
- Cloud NLP using Wit.ai
- Low-power ESP32 architecture
- Relay-based appliance control
- Extendable to multiple appliances

---

# System Architecture

```text
                User Voice
                     │
                     ▼
         INMP441 Digital Microphone
                     │
                     ▼
                  ESP32
                     │
               Wi-Fi Transfer
                     │
                     ▼
                Wit.ai API
          (Speech + Intent Recognition)
                     │
                     ▼
                  ESP32
                     │
                     ▼
              Relay Module
                     │
                     ▼
              Room Lighting
```

---

# Motivation

Commercial voice assistants such as Alexa and Google Assistant are powerful but expensive and privacy dependent.

This project explores:

- Low-cost alternatives
- Embedded AI and IoT integration
- Speech recognition pipelines
- Smart home automation
- Cloud vs Edge AI trade-offs

---

# Hardware Components

| Component | Function |
|----------|---------|
| ESP32 | Main microcontroller |
| INMP441 | Digital I2S microphone |
| Relay Module | Appliance switching |
| Wit.ai | Speech recognition |
| Wi-Fi | Cloud communication |

---

# Platform Evaluation

The following platforms were evaluated before implementation:

| Criteria | ESP32 | Raspberry Pi |
|---------|------|--------------|
| Power Consumption | Low | High |
| Wi-Fi/Bluetooth | Built-in | Built-in |
| Boot Time | <1 sec | ~30 sec |
| Complexity | Lightweight | Overkill |
| Cost | Low | Moderate |

**ESP32 was selected due to its low power consumption, fast boot time and suitability for embedded IoT applications.**

---

# Voice Processing Approaches

Two approaches were explored:

## 1. Local TinyML

### Advantages

- No internet dependency
- Very low latency
- Privacy preserving

### Limitations

- Fixed keywords only
- Requires labelled datasets
- Lower accuracy in noisy environments
- Model training complexity

---

## 2. Cloud NLP (Selected)

### Advantages

- Natural language understanding
- High recognition accuracy
- No on-device training
- Easily extensible

### Limitations

- Requires Wi-Fi
- Small network latency

**Selected:** Wit.ai based cloud speech processing.

---

# Current Progress

### Phase 1 — Hardware Fundamentals

- Traffic Light System
- Reaction Speed Game
- LED Patterns and Sensor Interfacing

### Phase 2 — Component Evaluation

- ESP32 vs Raspberry Pi comparison
- Microphone selection
- Analog vs Digital audio analysis

### Phase 3 — Voice Processing Architecture

- TinyML feasibility study
- Cloud NLP evaluation
- Wit.ai integration planning

### Phase 4 — System Design

- End-to-end architecture finalized
- Hardware stack finalized

---

# Next Steps

- [ ] Implement I2S audio capture on ESP32
- [ ] Integrate Wit.ai API
- [ ] Build relay switching circuit
- [ ] Perform end-to-end testing
- [ ] Measure latency and accuracy
- [ ] Improve noise robustness
- [ ] Final demonstration

---

# Documentation

Detailed 15-day progress report:

[SURGE099 Progress Report](docs/SURGE099_15 days Progress_Report.pdf)

---

# Author

**Abhishek Mehta**

B.Tech Electrical Engineering  
Indian Institute of Technology Delhi

---

### If you find this project interesting, feel free to ⭐ the repository!
