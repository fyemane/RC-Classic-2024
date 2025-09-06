# BCIT RC Classic 2024 – Competition Vehicle Documentation  

## 1. Introduction  
This document provides an overview of the vehicle prepared and entered into the **BCIT RC Classic 2024** competition. The vehicle was entered into three events:  
- Obstacle Course  
- Racing  
- Sumo  

The project objective was to enhance a commercially available RC platform through hardware and control system modifications to improve versatility and user control.  

---

## 2. Base Platform  
- **Model:** HYPER GO H16PL 1/16 RTR Brushless RC Buggy  
- **Key Specifications:**  
  - Maximum Speed: 62 km/h  
  - Drive System: 4WD with brushless motor  
  - Power Supply: 2S 2000 mAh LiPo battery  
  - Scale: 1/16  

The platform was selected for its speed, durability, and adaptability to custom modifications.  

---

## 3. System Modifications  

### 3.1 Hardware Modifications  
- Removed the stock RC transmitter/receiver system.  
- Integrated an **ESP32 microcontroller** to serve as the central control unit.  
- Configured the ESP32 to directly interface with the car’s electronic speed controller (ESC) and steering servo.  

### 3.2 Controller Integration  
- Replaced the default handheld RC controller with an **8BitDo Ultimate Bluetooth Controller**.  
- Established communication between the 8BitDo controller and the ESP32 via **Bluetooth**.  
- Utilized the **Bluepad32 architecture** in the Arduino environment to process and map controller inputs to motor and steering outputs.  

**Control Signal Flow:**  
8BitDo Controller → Bluetooth → ESP32 (Bluepad32) → ESC & Steering Servo

---

## 4. Competition Performance  

### 4.1 Obstacle Course  
- Achieved smooth navigation through complex turns due to precise input handling.  
- Demonstrated improved control responsiveness compared to the stock transmitter system.  

### 4.2 Racing  
- Maintained high-speed performance (~62 km/h) with consistent stability.  
- Control precision allowed for efficient cornering and acceleration.  

### 4.3 Sumo  
- Quick directional response provided a competitive advantage in pushing maneuvers.  
- 4WD drivetrain supported strong traction and maneuverability.  

---

## 5. Future Development  
The following improvements were identified for potential future iterations:  
- Incorporation of telemetry feedback (e.g., speed, battery voltage, and motor temperature).  
- Implementation of autonomous driving modes using onboard sensors and pathfinding algorithms.  
- Reduction of Bluetooth input latency through firmware optimization.  

---

## 6. Acknowledgements  
This project utilized the following hardware and software resources:  
- **Vehicle Platform:** HYPER GO H16PL Buggy  
- **Microcontroller:** ESP32 Development Board  
- **Controller:** 8BitDo Ultimate Bluetooth Controller  
- **Software Environment:** Arduino IDE with Bluepad32 library  
