# 🧠 Firmware Structure

Code is written using Arduino IDE or PlatformIO.

---

## 📁 Folder Structure

firmware/
│
├── src/
│   └── main.cpp              # 🎯 Main firmware entry point
│
├── include/
│   └── config.h              # ⚙️ Global constants, pin definitions, macros
│
├── lib/
│   └── sensor/
│       ├── SensorArray.cpp   # 🧪 Sensor array logic
│       └── SensorArray.h     # 📘 Sensor array header
│
├── platformio.ini            # 🛠️ PlatformIO config file (or .ino sketch if using Arduino IDE)
│
└── README.md                 # 📄 Documentation for firmware module

---

## 🔧 Features

- 🚗 **PID Line following**
  - 🔀 Intersection detection  
  - ⚡ Speed boost on straight lines  
  - ➖ Dashed-line crossing  

- 🎛️ **Calibration routine** (with buzzer/LED)  
- 🧭 **Mode switch** for maze mode  
- 📡 **Bluetooth/UART debug** (optional)  
- 🔋 **Battery low warning** 
