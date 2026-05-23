# 🚗 CAN-Based Vehicle Safety & Monitoring System using LPC2129

---

# 📌 Project Overview

This project implements a **CAN-Based Vehicle Safety & Monitoring System** using the **LPC2129 ARM7 Microcontroller**.

The system is designed for automotive applications where multiple nodes communicate using the **Controller Area Network (CAN) Protocol** for real-time monitoring and safety operations.

The project includes:

- Engine Temperature Monitoring
- Reverse Obstacle Detection
- CAN-Based Multi-Node Communication
- Vehicle Indicator Control
- LCD Dashboard UI
- Real-Time Warning Alerts

---

# 🎯 Project Aim

To design and develop an automotive safety and monitoring system using the **CAN Protocol**, where a central node monitors engine temperature, controls vehicle indicators, and processes reverse sensor data to provide real-time safety alerts.

---

# 🖼 Block Diagram

<img width="1026" height="707" alt="Block Diagram" src="https://github.com/user-attachments/assets/d94aad62-9c2c-4a5d-be80-d19869d6b7ec" />

---

# 🏗 System Architecture

## 🔹 Main Node
- Reads Engine Temperature
- Controls LCD Dashboard
- Sends Indicator Commands
- Receives Reverse Alerts

<img width="400" height="200" alt="image" src="https://github.com/user-attachments/assets/38ae6750-d8e7-4112-8ea5-6dc5721eb14f" />


## 🔹 Indicator Node
- Controls Left/Right Indicators
- Receives CAN Commands

## 🔹 Reverse Alert Node
- Reads Ultrasonic Sensor Data
- Sends Obstacle Alerts to Main Node

---

# ⚙ Hardware Requirements

| Component | Description |
|---|---|
| LPC2129 | ARM7 Microcontroller |
| MCP2551 | CAN Transceiver |
| HC-SR05 | Ultrasonic Sensor |
| DS18B20 | Temperature Sensor |
| 20x4 LCD | Display Unit |
| LEDs | Indicator Simulation |
| Buzzer | Warning Alert |
| Switches | External Interrupts |
| USB-UART | Programming Interface |

---

# 💻 Software Requirements

- Embedded C
- Keil uVision
- Flash Magic
- Proteus Simulation

---

# 📂 Repository Structure

```text
CAN-Based-Vehicle-Safety-Monitoring-System
│
├── Main_Node
├── Indicator_Node
├── Reverse_Alert_Node
│
├── Drivers
│   ├── LCD
│   ├── CAN
│   ├── Ultrasonic
│   ├── DS18B20
│   └── Delay
│
├── Proteus_Simulation
├── Circuit_Diagrams
├── Images
├── Documentation
│
├── README.md
└── LICENSE
