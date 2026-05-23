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

<table align="center">
<tr>

<td align="center">
<h2>🟢 SAFE</h2>
<img width="400" height="200" alt="vechicle_dashboard_main_node" src="https://github.com/user-attachments/assets/be15817f-cc5a-4c0d-aa08-35aa47366faf" />

<td align="center">
<h2>🟡 WARM</h2>
<img width="400" height="200" alt="Warm_condition" src="https://github.com/user-attachments/assets/ceb1934e-66a0-4a83-b69b-03b2b6e56021" />
</td>

</tr>
</table>

<h2 align="center">🔴 HOT / OVERHEATED</h2>

<p align="center">
<img width="400" height="200" alt="Hot_condition" src="https://github.com/user-attachments/assets/6e351198-8f4d-4dfa-85ff-63b9042f3fad" />
<img width="400" height="200" alt="Over_heated" src="https://github.com/user-attachments/assets/6588d404-9fb1-492e-9576-d1bcea9d9d25" />
   
<h2 align="center">⬅ LEFT INDICATOR</h2>

<p align="center">
<img width="400" height="200" alt="Left_indicator" src="https://github.com/user-attachments/assets/0c7a9174-2c1a-47fc-be2b-2ba782d46eb8" />
<img width="400" height="200" alt="Left_indicator_1" src="https://github.com/user-attachments/assets/b656e071-410e-47d8-a59e-f67f79f2ca11" />

<h2 align="center">➡ RIGHT INDICATOR</h2>

<p align="center">
<img width="400" height="200" alt="Right_indicator" src="https://github.com/user-attachments/assets/b82949ab-9ffa-499d-b71e-abfa1f72ae8e" />
<img width="400" height="200" alt="Right_Indicator_1" src="https://github.com/user-attachments/assets/35980e2c-7c80-4609-b6b9-3624a51669e4" />
<br><br>
<h2 align="center">🚗 Receives Reverse Alerts 🚗</h2>
<br><br>

<table align="center">
<tr>

<td align="center">
<h2>🟢 PATH CLEAR</h2>
<img width="400" height="200" alt="Reverse mode Path is clear" src="https://github.com/user-attachments/assets/cf3eadc1-045b-458d-ba36-b16e04eca415" />
</td>

<td align="center">
<h2>⚠ OBJECT NEARBY</h2>
<img width="400" height="200" alt="Object nearby" src="https://github.com/user-attachments/assets/cb3b5340-6aa5-4570-a5dd-beb452075ff7" />

</td>

</tr>
</table>

---

<h2 align="center">🚨 OBJECT DETECTED</h2>

<p align="center">
<img width="400" height="200" alt="Object detected" src="https://github.com/user-attachments/assets/8bc551ca-0790-4297-991f-1fad2d9dc8e6" />
<img width="400" height="200" alt="Warning  vehicle" src="https://github.com/user-attachments/assets/ee11257d-aa79-4c3d-b6e1-44778d4b57b3" />

</p>  

## 🔹 Indicator Node
- Controls Left/Right Indicators  
- Receives CAN Commands  

---

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
```

---

# ✅ Advantages

- Real-Time Vehicle Monitoring  
- Reliable CAN-Based Communication  
- Improved Vehicle Safety System  
- Modular Multi-Node Architecture  
- Low Latency Data Transmission  
- Efficient Temperature Monitoring  
- Reverse Collision Warning Support  
- Easy Integration with Automotive Systems  
- Scalable for Future Vehicle Features  
- User-Friendly LCD Dashboard Interface  

---

# 👨‍💻 Author

**Balaji Sai Kumar Mangena**  
*Embedded Systems Enthusiast*  

Passionate about Embedded Systems, Firmware Development,  
and Automotive Embedded Technologies.
