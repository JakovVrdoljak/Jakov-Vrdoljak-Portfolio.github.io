## 🔥 Project Overview: USB-Powered Cup Heater

Most commercial cup heaters rely on wall adapters that provide higher current and voltage than what standard USB ports can deliver. This project explores the design of a compact cup heater that operates on **USB power**, while working around its inherent power limitations.

### 💡 Key Idea
USB ports — especially from laptops — often cannot deliver enough sustained current for meaningful heating. To solve this, the project introduces an **external battery pack** that:
- **Powers the heating element directly** (bypassing USB limitations)
- **Charges via USB** when the heating element is off

This setup allows the heater to remain **USB-connected for convenience**, but still deliver enough energy for practical warming performance.

---

### 🧩 System Design Summary

| Component           | Function                                              |
|---------------------|--------------------------------------------------------|
| USB Input           | Powers logic and charges battery                       |
| Battery Pack        | Provides high current to the heating element           |
| Heating Element     | Converts electrical energy into heat                   |
| Switch Circuit      | Ensures the heater draws power only when battery is in use |

## 🔧 Design Details

This USB-powered cup heater combines charging, power delivery, and thermal control into a single compact PCB. The design uses a **battery + USB hybrid** approach to ensure safe heating without exceeding USB current limits.

---

### 🔋 Power Architecture

| Component     | Role                                                    |
|---------------|----------------------------------------------------------|
| **Battery**   | LP03448 Li-Po cell (3.7V, 1000 mAh)                       |
| **Charger IC**| RT9526A – USB-powered Li-ion/LiPo battery charger        |
| **USB Input** | Provides 5V for charging and sensing circuit (not heater)|
| **Output Control** | Heater powered from battery only, switched via BJT  |

---

### 🌡️ Temperature Sensing and Control

Temperature is controlled using a **PTC thermistor**, a **potentiometer** to set the desired heat threshold, and an op-amp used as a **comparator**. The comparator output drives a **BJT power switch** to enable or disable the heater based on surface temperature.

| Function            | Implementation                                      |
|---------------------|------------------------------------------------------|
| **Temp Sensor**     | PTC thermistor placed near heating element           |
| **Reference Adjust**| Potentiometer provides voltage threshold             |
| **Comparator**      | Op-amp compares temp signal to threshold             |
| **Power Switch**    | 2SD2657TL NPN BJT toggles heater ON/OFF              |

---

### ⚙️ Functional Logic

1. USB (5V) → charges battery via RT9526A.
2. Battery output is **disconnected from heater** during charging.
3. When not charging, BJT allows current to heater **only if**:
   - Temp < threshold (from potentiometer)
4. Once temp is reached, comparator disables BJT → heater off.

---

