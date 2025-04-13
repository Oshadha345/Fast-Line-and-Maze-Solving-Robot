# ⚡ Fast-Line + Maze Solving Robot 🤖  
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)  
[![Python 3.8+](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)  

---

## 📚 Overview  
A fast, intelligent line-follower robot for competitions using **ESP32**, **QRE sensors**, and **DRV8833 motor drivers**.

---

## 🏁 Competition Structure  

- 🌀 **Phase 1**: Advanced Line-Following Challenge  
  Designing a robot to navigate tracks with curves, sharp turns, dashed lines, and ramps.  

- 🧭 **Phase 2**: Autonomous Maze Navigation  
  If selected for finals, upgrade the robots with **AI** for maze-solving, route optimization, and quick decision-making.

---

## 🧠 Project Goals  

- 🧩 Modular design (easy upgrades)  
- ⚙️ ESP32-based for real-time performance  
- 📝 Fully documented hardware and firmware  
- 🐣 Beginner-friendly setup  

---

## 🌟 Features  

- 🎯 12-sensor PID-controlled analog line following  
- 🛠️ Custom PCB, boost/buck regulated  
- 🔄 Modular, upgradable to maze solver  

---

## 🔧 Hardware  

- 🧠 **ESP32-WROOM**  
- 🔌 **DRV8833** motor drivers  
- 👁️‍🗨️ **QRE1113** sensor array  
- 🧾 Custom PCB via **EasyEDA**  

---

## 🚀 Firmware  

- 🧬 Line following logic  
- 🎚️ PID tuning  
- 🔊 Status **LED** + **Buzzer** alerts  

---

## 🧰 Tools  

- 🧪 **EasyEDA**  
- 🧠 **Arduino IDE** *(or PlatformIO)*  
- 🏭 **JLCPCB** for manufacturing  

---

## 🗂️ Repo Structure  

- `hardware/`: 📐 Schematics, PCB files  
- `firmware/`: 💻 Arduino code & PID logic  
- `docs/`: 📄 Setup and usage guides  

---

## 📖 Documentation  

- [`docs/pcb_build_setup.md`](docs/pcb_build_setup.md): 📐 PCB & layout planning  
- [`docs/power_plan.md`](docs/power_plan.md): 🔋 Battery & voltage management  
- [`docs/sensor_array.md`](docs/sensor_array.md): 🧭 Sensor geometry & logic  
- [`docs/firmware_structure.md`](docs/firmware_structure.md): 💻 Arduino code setup  
- [`docs/soldering_guide.md`](docs/soldering_guide.md): 🔧 PCB assembly tips  
- [`docs/hardware_setup.md`](docs/harware_setup.md): ⚙️ Motors, regulators, and components  

---

## 📷 Gallery  
![PCB Image](hardware/PCB-Top.jpg)  

---

## 👨‍🔧 Maintainers  

- **Hardware**:  
  🧠 Oshadha Samarakoon  
  🛠️ Mokshika Herath  
  ⚡ Loshitha Udana  
  🔩 Dineth Perera  
  🧰 Themiya Wijekoon  

- **Firmware**:  
  💻 Fikry Nuhuman  
  🤖 Shihara Dewagedara  

- **Docs**:  
  📖 Oshadha Samarakoon  
