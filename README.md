# 🚨 IoT-Based Underground Cable Fault Distance Locator

![Platform](https://img.shields.io/badge/Platform-ESP32-blue)
![Domain](https://img.shields.io/badge/Domain-PowerSystems-orange)
![IoT](https://img.shields.io/badge/IoT-Enabled-green)
![Monitoring](https://img.shields.io/badge/System-FaultDetection-red)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)


## 📌 Overview
The **IoT-Based Underground Cable Fault Distance Locator** is designed to detect faults in underground power cables and estimate the distance of the fault from the source using electrical measurements.

The system uploads fault data to a cloud dashboard, enabling remote monitoring of cable health in smart power grids.

## 🎯 Objectives
- Detect cable short/open circuit faults  
- Estimate fault distance using voltage measurement  
- Display results locally and on cloud  
- Provide a scalable smart grid monitoring solution  

## 🛠️ Hardware Components
- ESP32 / Arduino UNO  
- Resistor network to simulate cable  
- Relay module / switch for fault creation  
- Breadboard & jumper wires  
- Optional LCD display  

## 💻 Software Used
- Arduino IDE  
- Embedded C / Arduino Programming  
- ThingSpeak / Firebase IoT dashboard  
- Serial Monitor Debugging  

## ⚙️ Working Principle
1. Underground cable is modeled using a resistor chain.  
2. Fault is introduced using a switch/relay.  
3. Voltage drop is measured by microcontroller.  
4. Distance is calculated using proportional method.  
5. Fault location is displayed locally.  
6. Data is uploaded to cloud dashboard.

## 🔌 Code Snippet
int raw = analogRead(ANALOG_PIN);
float voltage = (raw / 4095.0) * 3.3;
float distance = (voltage / 3.3) * TOTAL_LENGTH;
Serial.println(distance);

🌍 Applications
- Smart power grid monitoring
- Underground cable maintenance
- Electrical utility fault detection
- Industrial power distribution systems

🚀 Future Scope
- AI-based fault prediction
- Mobile monitoring app
- Real cable impedance modeling
- Multiple cable line monitoring
- GIS-based fault visualization
