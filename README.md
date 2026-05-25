# ThermaVault PID

**Industrial-style PID-controlled annealing oven conversion based on a Breville convection oven platform.**

ThermaVault PID is a documentation-first appliance conversion project focused on creating a more stable, serviceable, and repeatable annealing oven for engineering plastics used in 3D printing.

The build replaces the factory appliance timer/control behavior with an industrial PID controller, solid state relay heater control, high-temperature sensing, upgraded insulation, and a more modular electronics layout.

> **Status:** Active build / documentation in progress  
> **Platform:** Breville convection oven conversion  
> **Use case:** Controlled annealing cycles for 3D printed engineering plastics

<p align="center">
  <img width="720" alt="ThermaVault oven build" src="**https://github.com/user-attachments/assets/534b35a8-9bc2-4163-81de-b93c42fc987d**" />
</p>

---

## Table of Contents

- [Project Goals](#project-goals)
- [System Overview](#system-overview)
- [Documentation](#documentation)
- [Bill of Materials](#bill-of-materials)
- [Photos](#photos)
- [Safety Notice](#safety-notice)
- [License](#license)

---

## Project Goals

ThermaVault is being built as a compact process oven platform with a focus on:

- Stable annealing temperatures
- Reduced thermal overshoot
- Better chamber temperature consistency
- Programmable ramp/soak heat cycles
- Serviceable wiring and component layout
- Industrial-style process control hardware
- Improved insulation for long-duration heat stability
- Reusable appliance platform for future refinement

This is not meant to be a quick “add a PID and call it good” project. The goal is to build a cleaner, safer, better-documented oven conversion that can be maintained, upgraded, and understood later.

---

## System Overview

At a high level, the oven uses a PID controller to read chamber temperature and control the heating elements through a properly rated AC solid state relay.

The factory convection fan is retained so the oven can continue circulating hot air through the chamber. Temperature feedback is handled by a high-temperature sensor mounted for chamber/process temperature control.

<p align="center">
  <img width="420" alt="PID controller" src="https://github.com/user-attachments/assets/1f51fc1a-f9c9-4be2-b712-107a3e9f7998" />
  <img width="380" alt="SSR hardware" src="https://github.com/user-attachments/assets/84f70611-4241-4cf7-9cf8-10e8b605c220" />
</p>

---

## Documentation

| Document | Purpose |
|---|---|
| [Bill of Materials](./BOM.md) | Current parts list, links, quantities, and notes |
| [Safety Notes](./SAFETY.md) | Mains voltage, SSR, fuse, and thermal safety notes |
| [Tear Down Photo Log](./Build%20Photos/Tear%20Down%20Overview.md) | Documentation of the factory oven teardown process |
| [Build Log](./Build%20Photos/Build%20Log.md) | Ongoing build progression, thermal modifications, wiring integration, and control system development |

---

## Bill of Materials

The BOM has been moved to a dedicated file so it can expand without cluttering the main README.

See: **[BOM.md](./BOM.md)**

---

## Photos

Current photo documentation:

- [Tear Down Photo Log](./Build%20Photos/Tear%20Down%20Overview.md)
- [Build Log](./Build%20Photos/Build%20Log.md)

---

## Safety Notice

> **Warning:** This project involves mains AC voltage, high temperatures, resistive heating elements, appliance modification, and long-duration unattended heat risk. Mistakes can cause electric shock, fire, equipment damage, or injury.

Minimum safety expectations:

- Use properly rated fuses or breakers.
- Maintain chassis ground continuity.
- Use high-temperature wire inside hot zones.
- Mount the SSR to a correctly sized heat sink.
- Keep low-voltage and mains-voltage wiring separated.
- Use strain relief on incoming power.
- Do not bypass factory thermal safety devices unless they are replaced with equal or better protection.
- Verify wiring with a meter before applying power.
- Perform initial heat tests attended and away from flammable material.

Read the full safety page before copying any part of this build: **[SAFETY.md](./SAFETY.md)**

---

## License

This project is licensed under the **GNU GPL v3.0 License**.

---

## FishyFabsPNW

Designed, built, and documented by **FishyFabsPNW**.
