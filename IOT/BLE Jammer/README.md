# BLE Jammer — IoT & Hardware Security Research

**Research Areas:** BLE Security · IoT Security · Embedded Systems · Hardware Hacking

**Hardware Platform:** ESP32 and two nRF modules

**Project Status:** Prototype developed; technical documentation and further research ongoing.

---

## Project Overview

This project documents my independent exploration of wireless security through the development of a BLE jammer prototype using an ESP32 and two nRF modules.

My objective was to explore the relationship between embedded hardware, wireless communication, and the security challenges associated with connected devices.

The project represents an important step in my journey toward IoT security and hardware hacking. It has encouraged me to investigate wireless communication fundamentals, device architecture, and the importance of availability in connected systems.

## Hardware Platform

The prototype incorporates the following components:

| Component | Role in the Project |
|---|---|
| ESP32 | Microcontroller platform |
| nRF module 1 | Wireless hardware component |
| nRF module 2 | Wireless hardware component |

The precise functions of the nRF modules depend on their models, firmware, configuration, and the way they are integrated into the prototype.

## Research Motivation

I wanted to explore wireless security beyond theoretical concepts and develop a better understanding of how hardware and wireless communication interact.

Building this prototype motivated me to investigate wireless availability, communication reliability, and the security implications of connectivity disruption.

It also encouraged me to look beyond the prototype itself and consider how IoT developers can design devices that respond safely to communication failures.

## Security Context

Bluetooth Low Energy (BLE) is widely used in wearable devices, smart home systems, sensors, and other IoT applications.

Wireless communication can be affected by environmental interference, hardware limitations, configuration issues, and deliberate interference.

These conditions may result in packet loss, connection instability, or reduced availability.

It is important to distinguish physical-layer radio interference from protocol-level vulnerabilities and implementation weaknesses because they require different assessment and mitigation approaches.

## Research Questions

- How do BLE-enabled devices handle unexpected connectivity loss?
- What factors influence wireless communication reliability?
- How can connected devices recover safely from communication failures?
- What security properties are provided by BLE pairing and encryption?
- How can developers improve the resilience of connected devices?

## Future Research

My next learning objectives include:

- BLE protocol analysis.
- Embedded systems and microcontroller security.
- Firmware analysis.
- Hardware debugging interfaces.
- IoT threat modeling.
- Defensive wireless security.
- Secure device recovery and resilience.

## Responsible Research

This project is documented for educational and defensive security research.

Active radio-frequency interference may affect nearby devices and may be restricted by applicable regulations. Any further testing should be appropriately authorized and conducted within lawful, controlled conditions.

Experimental results will be documented separately and supported by evidence.

## References

- [Bluetooth Core Specification](https://www.bluetooth.com/specifications/specs/)
- [NIST IoT Cybersecurity Guidance](https://csrc.nist.gov/pubs/ir/8259/final)
- [OWASP Internet of Things Project](https://owasp.org/www-project-internet-of-things/)

## About This Project

This prototype represents part of my ongoing journey into IoT security and hardware hacking.

I am interested in understanding how embedded devices operate, how wireless communication works, and how security researchers can help make connected systems more resilient.

**Learn. Build. Investigate. Document.**
