#  ThermaVault PID

Industrial-style PID-controlled annealing oven conversion based on a Breville convection oven platform.

Designed for engineering plastics requiring controlled annealing cycles, improved thermal consistency, and long-duration stability.

---

#  Project Overview

ThermaVault PID is a custom annealing oven conversion focused on improving chamber stability, airflow consistency, and programmable process control using industrial-style hardware.

The project replaces the factory timer/controller system with:

- Industrial PID temperature control with  Programmable ramp/soak heat cycles -<img width="566" height="624" alt="image" src="https://github.com/user-attachments/assets/1f51fc1a-f9c9-4be2-b712-107a3e9f7998" />

- SSR-based heater switching -<img width="640" height="640" alt="image" src="https://github.com/user-attachments/assets/231521ba-c5fa-4c40-af27-a3a464f714a6" />


The goal is to create a reusable and serviceable process oven platform for annealing engineering plastics.

---

#  Design Goals

- Stable annealing temperatures
- Reduced thermal overshoot
- Better chamber temperature consistency
- Industrial-style process control
- Reusable appliance platform
- Modular and serviceable electronics
- Long-duration operation reliability
- Expandable hardware ecosystem

---

# ⚠️ Safety Notice

This project involves:

- Mains AC voltage
- High temperatures
- Resistive heating elements
- Solid state relays
- Appliance modification

This repository is intended for educational and informational purposes only.

Always:

- Use proper grounding
- Use correctly rated wire ( Mica Perferred )
- Use thermal protection
- Use proper fuse protection
- Keep SSRs heatsinked ( With Thermal Paste!!)
- Verify wiring before applying power
- Keep electronics isolated from heat

DO NOT bypass thermal safety devices.

---

#  System Overview

The oven is controlled using an industrial PID controller driving AC heater loads through a zero-cross SSR.

The factory convection fan is retained to improve:

- Chamber airflow
- Thermal consistency
- Temperature recovery
- Heat distribution
- 
---

# 🔧 Hardware Overview

| Component | Description |
|---|---|
| Oven Platform | Breville convection oven |
| PID Controller | Industrial modular PID controller |
| Heater Control | Industrial AC SSR |
| Temperature Sensor | RTD PT100 |
| Airflow | Factory convection fan |
| Safety Devices | Thermal cutoff + fuse protection |

---

# Recommended SSR Specifications

The heater system is designed around an industrial AC zero-cross SSR intended for resistive heating loads.

Recommended SSR specifications:

- AC output SSR
- Zero-cross switching
- 25A–40A current rating
- 3–32VDC control input
- Chassis/heatsink mount
- Designed for resistive heater loads

Recommended industrial SSR brands include:

- Sensata-Crydom -(https://www.digikey.com/en/products/detail/sensata-crydom/D2440/221764)
- Celduc -(https://www.digikey.com/en/products/detail/celduc/SO943460/14311190)
- Panasonic Electric Works -(https://www.digikey.com/en/products/detail/panasonic-industry/AQA611VL/2364686)
- Crouzet -(https://www.digikey.com/en/products/detail/crouzet/84137670N/13175923)
  
---

# 📷 Photos

Project photos, wiring diagrams, and build documentation will be added as the project progresses.

---

#  License

This project is licensed under the GNU GPL v3.0 License.
---

#  FishyFabsPNW

Designed and documented by FishyFabsPNW.
