# 🚨 Motion Detection Alarm System (Prototype)

![Banner](asset/banner.png)

> A simple ESP32-based motion detection system that triggers a buzzer alert when motion is detected.

---

## 📌 Overview

This project is a **basic prototype (Phase 1)** of a motion detection system using an ESP32 microcontroller.

The system detects motion using a PIR sensor and responds by activating a buzzer while also displaying status messages in the Serial Monitor.

---

## ⚡ Features

- Detects motion using PIR sensor  
- Activates buzzer with blinking alert pattern  
- Displays real-time status via Serial Monitor  
- Simple and efficient hardware-based system  

---

## 🔧 Hardware Components

- ESP32  
- PIR Motion Sensor  
- Active Buzzer  
- Jumper Wires  

---

## 🔌 Pin Configuration

| Component   | GPIO Pin | Type   |
|------------|---------|--------|
| PIR Sensor | 14      | Input  |
| Buzzer     | 27      | Output |

---

## ⚙️ Working Principle

1. The PIR sensor continuously monitors motion  
2. ESP32 reads the sensor value using digital input  
3. If motion is detected (HIGH):
   - Serial prints **"Motion Detected!"**  
   - Buzzer turns ON and OFF repeatedly (alert pattern)  
4. If no motion (LOW):
   - Serial prints **"No Motion"**  
   - Buzzer remains OFF  

---

## 💻 Code Structure

### 🔹 setup()
- Configures PIR pin as **INPUT**  
- Configures buzzer pin as **OUTPUT**  
- Starts Serial communication (115200 baud rate)  

### 🔹 loop()
- Continuously reads PIR sensor value  
- Triggers buzzer alert when motion is detected  
- Maintains system behavior in real-time  

---

## 🔊 Output Behavior

| Condition        | Output                          |
|----------------|---------------------------------|
| Motion Detected | Buzzer beeps (ON/OFF pattern)   |
| No Motion       | Buzzer OFF                      |

---

## ▶️ Installation & Usage

1. Connect components according to pin configuration  
2. Upload the code to ESP32  
3. Open Serial Monitor (baud rate: **115200**)  
4. Observe system behavior:
   - Motion → Alert  
   - No Motion → Idle  

---

## 🚀 Future Scope (Next Version)

> *(Not included in this prototype)*

- WiFi connectivity  
- Real-time mobile notifications  
- Cloud/API integration  
- Camera module (ESP32-CAM)  

---

## 📖 Notes

- This is an **initial prototype** focusing on core functionality  
- Designed as a foundation for a future smart IoT security system  

---

## 📜 License

This project is for educational purposes.
