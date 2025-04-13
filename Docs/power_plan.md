# 🔌Power Plan & Voltage Logic

This guide covers the power distribution and logic level planning for the robot.

---

## 🔋 Battery Setup


| 2S LiPo (7.4V) | Lower weight, ~ good for 6V motors |


⚠️ Always balance charge and include a **low-voltage buzzer** (set for 3.4V/cell cut-off).

---

## ⚡ Voltage Regulation

|📦 Component | ⚙️ Voltage |
|--------|-------|
| ESP32 WROOM   | 3.3V |
| Sensors (QRE1113GR)     |5V  |
| DRV8833 + Motors     | 6V+ |
| XL6009 Output     | 7.4–11.1V adjustable |


### 🔁 XL6009 Boost Regulator

- Input: 2S LiPo
- Output: 12V (adjustable with onboard pot)
- Add 470uF capacitor at output for motor surges

---

## 🔄 Voltage Conversion

### Sensor Logic (5V → 3.3V):

Use a **resistor divider**:

Vout = Vin × R2 / (R1 + R2)


For 5V → 3.3V:

- R1 = 2.2kΩ
- R2 = 3.3kΩ

Apply to each sensor output before ESP32.

Alternative: Use logic level shifter module if you prefer.

---

## 🔌 Switch & Charging Port

- Use a rocker switch on the main LiPo line.
- Add 2-pin JST port to access battery for charging.


