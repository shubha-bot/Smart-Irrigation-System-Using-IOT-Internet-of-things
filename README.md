# 🌱 Smart Irrigation System using ESP32 and IoT

A smart irrigation system that automatically monitors soil moisture and turns the water pump ON/OFF based on real-time data. Built using **ESP32**, soil moisture sensors, and integrated with **Blynk IoT** for remote monitoring and control.

---

## 📌 Project Information

- 🔖 **Project Title**: Smart Irrigation System using IoT
- 🎓 **Semester**: 3rd Semester (BCA)
- 🏫 **College**: Graphic Era University
- 👨‍🏫 **Mentorship**: Under the guidance of *Anmol Chaudhary*
- 👨‍💻 **Developed by**: **Shubham Raj**

---

## ✅ Features

- 🌡️ Real-time soil moisture monitoring
- 🌧️ Temperature and humidity data (optional with DHT11/DHT22)
- 💧 Automatically turns water pump ON when soil is dry
- 📲 Real-time data logging on Blynk IoT app
- 🔌 Wi-Fi connectivity via ESP32

---

## 🛠️ Hardware Requirements

| Component              | Quantity |
|------------------------|----------|
| ESP32 Dev Board        | 1        |
| Soil Moisture Sensor   | 1–2      |
| DHT11/DHT22 Sensor     | 1 (Optional) |
| Relay Module           | 1        |
| Water Pump             | 1        |
| Power Source (Battery/Adapter) | 1  |
| Jumper Wires           | As needed |
| Breadboard             | 1        |

---

## 🔌 Circuit Connections

- **Soil Moisture Sensor**
  - VCC → 3.3V (ESP32)
  - GND → GND
  - A0 → GPIO 34

- **Relay Module**
  - IN → GPIO 27
  - VCC → 3.3V / 5V
  - GND → GND

- **DHT11/DHT22 Sensor (Optional)**
  - VCC → 3.3V
  - GND → GND
  - DATA → GPIO 4

---

## 💻 Code Setup

- Open `SmartIrrigation.ino` in the Arduino IDE
- Install required libraries:
  - `Blynk`
  - `DHT sensor library`
  - `WiFi`
- Replace the following credentials in the code:
  ```cpp
  char auth[] = "Your_Blynk_Auth_Token";
  char ssid[] = "Your_WiFi_SSID";
  char pass[] = "Your_WiFi_Password";
