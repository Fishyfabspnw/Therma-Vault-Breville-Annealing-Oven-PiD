# ThermaVault PID — Safety Notes

## Warning

This project involves:

- Mains AC voltage
- High current heater loads
- Elevated temperatures
- Appliance modification
- Fire risk
- Long-duration heat cycles

If you are not comfortable working around mains wiring and electrical safety practices, do not attempt this build.

---

## Electrical Safety

### Grounding

The oven chassis must remain properly grounded.

Do not remove or defeat chassis grounding connections.

---

### Fuse / Breaker Protection

Incoming AC power should be protected by a properly sized fuse or breaker.

Protection should be installed before downstream electronics and heater circuits.

---

### SSR Safety

Solid state relays generate heat and can fail.

Minimum recommendations:

- Use a properly rated SSR
- Mount the SSR to a heat sink
- Ensure airflow if enclosure temperatures rise
- Verify wiring polarity and load routing
- Avoid counterfeit SSRs

---

### Wire Selection

Use properly rated high-temperature wire inside heated zones.

Do not use standard low-temperature hookup wire near heating elements.

---

### Wire Routing

Separate:

- Low-voltage sensor wiring
- PID control wiring
- High-voltage AC heater wiring

This helps reduce electrical noise and improves safety/serviceability.

---

## Thermal Safety

Recommended:

- Independent thermal cutoff
- Attended first heat tests
- Non-flammable mounting surface
- Clearance from combustible materials

Never leave early test cycles unattended.

---

## Build Responsibility

This repository is for documentation and educational purposes.

Anyone reproducing this project assumes responsibility for their own wiring, safety validation, thermal testing, and electrical compliance.
