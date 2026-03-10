# LM358 Heat-Activated Switch (Thermistor)

A temperature-sensitive control circuit utilizing the **LM358 IC**. This project acts as a thermal switch that triggers when a specific heat threshold is reached.

## 🚀 Overview
This project uses an **NTC (Negative Temperature Coefficient) Thermistor**. As temperature increases, the resistance of the thermistor decreases. The LM358 monitors this change and triggers a **HIGH** output when the temperature exceeds the user-defined limit set by the potentiometer.

### Features
* **High Sensitivity:** Detects small temperature fluctuations.
* **Threshold Control:** Adjustable trigger point via a 10k potentiometer.
* **Versatile Output:** Can be interfaced with a BC547 transistor to drive 9V relays.

## 🛠️ Bill of Materials (BOM)
| Component | Value | Purpose |
| :--- | :--- | :--- |
| **LM358 IC** | Dual Op-Amp | Comparator |
| **NTC Thermistor** | 10kΩ (@25°C) | Temperature Sensor |
| **Potentiometer** | 10kΩ | Temperature Threshold Set |
| **Resistor** | 10kΩ | Voltage Divider Fixed Resistor |
| **Resistor** | 220Ω | LED Current Limiter |
| **LED** | Red/Orange | Heat Indicator |

## ⚡ Connection Guide
1. **Power:** Pin 8 (+9V), Pin 4 (GND).
2. **Reference:** Potentiometer center pin to **Pin 6**.
3. **Sensor:** Thermistor to +9V, 10k Resistor to GND. Junction to **Pin 5**.
4. **Output:** LED (Anode) to **Pin 7**, Cathode to GND (via 220Ω).

## 🧪 Testing
Hold the thermistor between your fingers or bring a warm object near it. The LED should trigger once the threshold is crossed. Adjust the 10k pot to change how "hot" it needs to be to turn on.
