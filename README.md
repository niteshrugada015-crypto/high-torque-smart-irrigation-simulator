# High-Torque Smart Irrigation Simulator

An interactive engineering simulator for a **High-Torque Industrial Retrofit Smart Irrigation System** designed for remote monitoring, automatic irrigation control, and retrofit installation on existing agricultural irrigation infrastructure.

## 🌱 Project Overview

The system is designed for farms where replacing the existing irrigation pipeline is expensive or impractical. A **high-torque servo actuator** is installed on the existing field valve using a retrofit coupling.

The system continuously monitors soil moisture, valve status, power conditions, and communication status. Based on soil-moisture conditions, the controller can automatically open or close the irrigation valve.

The simulator demonstrates the complete operation of the proposed system, including **automatic irrigation, remote monitoring, solar power management, actuator protection, and fault detection**.

---

## 🎯 Objectives

- Automate irrigation using soil-moisture feedback.
- Retrofit existing irrigation valves without replacing the pipeline.
- Enable remote monitoring and valve control.
- Use solar energy for off-grid operation.
- Detect actuator stall and abnormal operating conditions.
- Monitor battery and power conditions.
- Provide real-time system status through a dashboard.
- Demonstrate the complete power, mechanical, and information flow.

---

## ⚙️ Main Components

| Component | Function |
|---|---|
| ESP32 Controller | Central processing and control |
| High-Torque Servo | Opens and closes the existing valve |
| Capacitive Soil-Moisture Sensor | Measures soil moisture |
| GSM Module | Remote communication |
| GPS Module | Location and timestamp information |
| MOSFET + Optocoupler | Electrical protection and switching |
| Stall Detection | Detects actuator overload/stalling |
| Solar Panel | Generates electrical power |
| Solar Charge Controller | Manages solar charging |
| LiFePO4 Battery | Stores electrical energy |
| Supercapacitor | Provides short-duration energy buffering |
| DC-DC Converter | Provides regulated voltage |
| IP67 Enclosure | Protects electronics from environmental conditions |

---

## 🔄 System Architecture

### Power Flow

```text
Solar Panel
     ↓
Solar Charge Controller
     ↓
LiFePO4 Battery + Supercapacitor
     ↓
DC-DC Voltage Regulation
     ↓
ESP32 Controller + Sensors + Servo Actuator
