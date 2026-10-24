# Bluetooth Low Energy Security Fundamentals

## Introduction

Bluetooth Low Energy (BLE) is a wireless communication technology designed for devices that require low power consumption and efficient short-range communication.

It is widely used in wearable technology, smart home devices, sensors, medical accessories, and embedded systems.

BLE provides a useful foundation for studying IoT security because its operation involves multiple layers, each with different responsibilities.

This document summarizes important BLE concepts and their security implications.

## 1. BLE Architecture

### Generic Access Profile (GAP)

GAP defines device discovery, advertising, connection establishment, and related communication procedures.

From a security perspective, these functions influence how devices become discoverable and establish relationships with other devices.

### Generic Attribute Profile (GATT)

GATT organizes application data into services and characteristics.

For example, a sensor may expose a service containing characteristics that represent measurements or device status.

Access restrictions and authorization decisions must be implemented appropriately for sensitive operations.

### Attribute Protocol (ATT)

ATT provides mechanisms for accessing and exchanging attribute data.

The security implications depend on how attributes are protected and how applications enforce access requirements.

### Link Layer

The BLE Link Layer manages low-level wireless communication, including advertising, connection events, and channel-related behavior.

Understanding this layer helps distinguish radio communication problems from application-level security issues.

## 2. BLE Communication Roles

### Central

A central device initiates or manages connections with peripheral devices.

### Peripheral

A peripheral device can advertise its availability and accept connections according to its configuration.

These roles describe communication responsibilities and should not be confused with security privileges.

A device's communication role does not automatically establish whether it is trusted or authorized.

## 3. BLE Security Properties

### Confidentiality

Confidentiality helps prevent unauthorized parties from reading protected information.

BLE encryption can contribute to this objective when appropriate security procedures are correctly implemented.

### Integrity

Integrity mechanisms help detect or prevent unauthorized modification of protected information.

The specific protections depend on the protocol mechanisms and implementation.

### Authentication

Authentication helps establish the identity or legitimacy of a communicating party.

Pairing configuration and application-level identity checks influence the security of a BLE implementation.

### Availability

Availability concerns whether devices and services remain usable when required.

Wireless interference can affect availability even when other security mechanisms operate correctly.

## 4. BLE Pairing and Bonding

Pairing establishes security information between devices using supported BLE procedures.

Bonding allows devices to retain appropriate security information for subsequent interactions.

Security depends on the pairing method, device configuration, user interaction, and implementation quality.

Developers should select suitable security settings for the device's threat model and intended use.

## 5. Wireless Availability Risks

BLE communication can be affected by:

- Environmental interference.
- Physical obstructions.
- Competing wireless activity.
- Antenna and hardware limitations.
- Device power problems.
- Firmware defects.
- Protocol implementation weaknesses.
- Deliberate radio-frequency interference.

These causes should not be treated as equivalent.

A security assessment should determine which explanation is supported by the available evidence.

## 6. Jamming Versus Protocol-Level Attacks

Radio-frequency jamming affects the physical transmission and reception of wireless signals.

Protocol-level attacks instead target weaknesses in communication procedures or device implementations.

Although both can cause communication disruption, their mechanisms and defensive requirements differ.

Encryption is not a general solution to radio-frequency interference.

Protocol weaknesses require appropriate implementation and configuration fixes, while availability resilience may require improved recovery behavior, monitoring, and alternative operational mechanisms.

## 7. BLE Security Assessment Questions

When assessing an authorized BLE device, consider:

1. What services and characteristics does the device expose?
2. Which operations require authentication?
3. Is sensitive information adequately protected?
4. Are device identity and privacy handled appropriately?
5. How does the device respond to unexpected disconnections?
6. Does the application handle missing or delayed data safely?
7. Are firmware updates and configuration changes protected?
8. Is the device's behavior consistent with its documented security requirements?

## 8. Learning Objectives

My next objectives are to understand BLE advertising, connection management, GATT services, pairing, authentication, and the relationship between protocol security and application-level authorization.

I also want to learn how to document BLE observations accurately and distinguish normal device behavior from potential security issues.

## References

- [Bluetooth Core Specification](https://www.bluetooth.com/specifications/specs/)
- [Bluetooth SIG](https://www.bluetooth.com/)
- [NIST IoT Cybersecurity Guidance](https://csrc.nist.gov/pubs/ir/8259/final)

---
