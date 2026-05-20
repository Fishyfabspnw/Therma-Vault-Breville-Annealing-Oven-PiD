#  ThermaVault PID

Industrial-style PID-controlled annealing oven conversion based on a Breville convection oven platform.

Designed for engineering plastics requiring controlled annealing cycles, improved thermal consistency, and long-duration stability.

---

#  Project Overview

ThermaVault PID is a custom annealing oven conversion focused on improving chamber stability, airflow consistency, and programmable process control using industrial-style hardware.

The project replaces the factory timer/controller system with:

- Industrial PID temperature control
- SSR-based heater switching
- Convection airflow management
- Programmable ramp/soak heat cycles
- Independent thermal safety systems

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

- Crydom
- Celduc
- Panasonic Industrial
- Crouzet

A detailed BOM with the exact hardware used in this build will be added later.

---

#  Temperature Sensing

The system currently uses:

- Single PID control thermocouple
- Chamber-air based temperature control

Probe placement is focused around:

- Center chamber positioning
- Part-height measurement
- Reduced direct radiant exposure

Additional monitoring probes may be added later for chamber thermal mapping and consistency testing.


---

# 📷 Photos

Project photos, wiring diagrams, and build documentation will be added as the project progresses.


---

#  Repository Status

 Active Development

This repository is continuously evolving as the project progresses through testing, tuning, and refinement.

---

#  Contributing

Suggestions, improvements, and thermal/process-control discussions are welcome.

---

#  License

This project is licensed under the GNU GPL v3.0 License.
---

#  FishyFabsPNW

Designed and documented by FishyFabsPNW.
