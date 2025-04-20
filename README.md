# 🏠 Home_Automation

[![Platform](https://img.shields.io/badge/Platform-ESP32-blue.svg)](https://www.espressif.com/)  
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

Welcome to the *Home Automation Dashboard*! This project transforms your ESP32 into a sleek, web‑based control center for monitoring temperature, humidity & motion and toggling relays in real time.  

---

## 📋 Table of Contents

- [✨ Features](#-features)  
- [📦 Hardware Requirements](#-hardware-requirements)  
- [⚙ Software Requirements](#-software-requirements)  
- [🔧 Wiring & Pinout](#-wiring--pinout)  
- [🚀 Installation & Usage](#-installation--usage)  
- [🌐 Web Interface](#-web-interface)  
- [🛠 Customization](#-customization)  
- [🤝 Contributing](#-contributing)  
- [📄 License](#-license)  

---

## ✨ Features

- 🎉 *Landing Page*: “Welcome to the Home Automation Dashboard”  
- 🖥 *Dashboard Menu*: 3 big buttons → Real‑Time Monitoring, Control Devices, Help  
- 📈 *Real‑Time Monitoring*:  
  - Live *Temperature* & *Humidity* charts (Chart.js)  
  - Auto‑updating via WebSocket (every 2 sec)  
- 🔌 *Control Devices*:  
  - Toggle *4 relays* (active LOW) from a modern UI  
- ❓ *Help Page*: Usage tips & troubleshooting  
- 📡 *WebSocket Server* on port *81* for ultra‑smooth updates  
- 🌡 *DHT11* temperature & humidity sensor  
- 🚶 *PIR* motion detection sensor  

---

## 📦 Hardware Requirements

- *ESP32 Development Board*  
- *DHT11* temperature & humidity sensor  
- *PIR Motion Sensor*  
- *4-channel Relay Module*  
- Jumper wires & breadboard / custom PCB  
- 5V power supply (or USB)

---

## ⚙ Software Requirements

- [Arduino IDE](https://www.arduino.cc/en/software) (≥ 1.8.15)  
- ESP32 Board Support installed  
- Libraries:  
  - DHT sensor library by Adafruit  
  - WebSocketsServer  
  - WebServer (built‑in)  
  - WiFi.h (built‑in)  

---

## 🔧 Wiring & Pinout

| Component     | ESP32 Pin |
|-------------- |----------:|
| DHT11 Data    | GPIO 4    |
| PIR Sensor    | GPIO 15   |
| Relay 0       | GPIO 16   |
| Relay 1       | GPIO 17   |
| Relay 2       | GPIO 18   |
| Relay 3       | GPIO 19   |
| GND / VCC     | GND / 3.3 V (or 5 V for relays) |

> *Tip:* Use a separate 5 V supply for the relays to avoid brown‑outs!

---

## 🚀 Installation & Usage

1. *Clone the repo*  
   ```bash
   git clone https://github.com/<your‑username>/Home_Automation.git
   cd Home_Automation
