# 🛠️ PCB Build Setup Guide

This guide walks you through building the PCB for our ESP32-based line follower robot.

---

## 🧩 Components & Connectors

| 🧱 Component         | 🔍 Description                            |
|---------------------|-------------------------------------------|
| ESP32 WROOM         | Main controller (3.3V logic)              |
| DRV8833 x2          | Dual motor drivers                        |
| QRE1113GR x12       | Reflective IR sensors                     |
| XL6009 Module       | Boost converter from 2S/3S LiPo           |
| JST 2.0 Connectors  | For motors and sensors (maintenance)      |
| Status LED          | Debugging status                          |
| Buzzer              | Low battery alert or debug tones          |
| Power Switch        | Toggle main supply                        |
| Charging Port       | JST connector for LiPo charging           |
| Voltage Divider     | For QRE sensors to ESP32 (5V → 3.3V)      |

---

## 📏 PCB Design Guidelines

- ✂️ **Custom cutout shape**: U-shaped for front sensor array  
- 📐 **Motor drivers** placed close to output pins for cleaner routing  
- ⚙️ **Sensor headers** aligned with front cutout  
- 🎯 **ESP32** centered with easy GPIO routing  
- 🔋 **Decouple** with 0.1uF caps near ICs  
- 🧵 Route thick traces for motor power lines  
- 🖊️ Add silkscreen labels for all pins  
- 🔩 Use 3.2mm mounting holes at 4 corners  

---

## 🖥️ EasyEDA Setup

1. 🌐 Open [https://easyeda.com](https://easyeda.com)
2. 🆕 Create a new Project: **ESP32 Line Follower**
3. 📥 Import libraries:
   - ESP32-WROOM  
   - DRV8833 motor drivers (2x)  
   - QRE1113GR sensors (12x)  
   - XL6009 boost converter  
   - Power switch (SPDT or slide switch)  
   - JST connectors for motors, sensors, battery  
   - Buzzer, optional OLED, and status LED  
4. ✏️ Draw schematic:
   - ESP32 center  
   - DRV8833 left/right  
   - Sensor headers bottom  
5. 🧩 Switch to **PCB Editor**
6. 🪚 Shape the board:
   - Use "Board Outline" tool  
   - Draw custom shape (e.g., rounded front, rectangular base)  
   - Add sensor mounting cutouts or silkscreen indicators  
7. 🤖 Auto-route, then manually adjust:
   - Use ground-plane techniques  
   - Ensure motor traces are wide (~1mm)  
8. ✅ Use **Design Manager** to fix DRC issues  
9. 👓 Preview in **3D View**
10. 📤 Export **Gerber files** for JLCPCB

---

## 🔁 Files to Export

- 📦 **Gerber** `.zip`  
- 📃 **BOM** `.csv`  
- 📍 **Pick and Place** `.csv` (optional for SMT)
