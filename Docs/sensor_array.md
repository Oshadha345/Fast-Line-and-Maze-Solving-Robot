# 📡 Sensor Array Guide

This document details the layout, logic, and integration of the IR sensor array.

---

## 🔧 Sensor Type: QRE1113GR

- 🔁 Reflective IR sensor  
- 📊 Analog or Digital output (**we use analog**)  
- 🔌 Connect: **VCC (5V)**, **GND**, **OUT**

---

## 📐 Layout & Positioning

| 📦 Sensor Count | 📍 Placement |
|-----------------|--------------|
| 🔢 12 (Recommended) | 11 Front, 1 Rear (for detecting straights and dashed-lines) |

### ➡️ Front Array

- 📏 Evenly spaced in a **slight arc**
- 🎯 Middle two placed closest to center line
- 🔄 Edge sensors **angled ~15° outward**

### 🔙 Back Sensor

- 🧭 Vertically aligned with middle front sensor  
- ⚠️ Used for **intersection detection** (dashed lines, T-junctions)

---

## 🛠️ Mounting Tips

- 📏 Ideal height: **3–5mm from the ground**
- 🖤 Use **black matte PCB** under sensors (reduces reflection noise)
- 🧪 Calibrate **sensor thresholds** in the firmware for best performance

---

## 🧠 ESP32 Connection

- 🔋 Each sensor **VCC = 5V** (from LDO regulator)
- 🌐 **GND = Common ground**
- 🧷 **OUT = To GPIO** (⚠️ with resistor voltage divider to step down 5V → 
