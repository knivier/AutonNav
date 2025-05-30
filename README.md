# AutonNav

## Modular RC Car Project

A self-driving, modular RC car designed for outdoor use and future expandability. This vehicle is capable of manual control via long-range radio communication and is planned to support autonomous features such as computer vision, LiDAR-based navigation, and wireless charging.

---

title: "Modular RC Car"
author: "Knvier (@knvier)"
description: "An outdoor modular RC car with future autonomous capabilities."
created\_at: "2024-03-20"

---

## Overview

This project is part of Hack Club's custom project initiative. The RC car is designed to be modular, capable of both manual and autonomous control. The system uses off-the-shelf components combined with custom code and hardware interfaces to create a flexible robotics platform.

## Goals

* Phase 1 (Under \$150):

  * Assemble chassis with motors and drivetrain
  * Integrate battery and power system
  * Setup long-range radio communication for manual remote control
  * Control vehicle via keyboard on remote computer

* Phase 2 (Under \$350):

  * Add Raspberry Pi or similar SBC
  * Integrate camera module and basic computer vision
  * Add LiDAR for obstacle detection
  * Implement basic path planning and route following
  * Build support for future wireless charging docking

## Hardware (Planned Bill of Materials)

### Phase 1 (\~\$150 Budget)

* RC car chassis (Traxxas-size compatible)
* 4x DC motors + motor driver
* Battery pack (Li-Ion or Li-Po)
* Radio communication module (e.g. NRF24L01+, HC-12, or LoRa)
* Arduino Uno/Nano or ESP32 microcontroller
* Power distribution board
* Wheels + rubber tires

### Phase 2 (Total <\$350)

* Raspberry Pi 4 or Zero 2 W
* USB or CSI camera
* LiDAR (e.g. RPLIDAR A1 or TF-Luna)
* Wireless charging coil module
* Voltage regulators and auxiliary electronics

## Software & Control

* Remote keyboard interface via PC
* Custom telemetry protocol for motor control and video feed
* Python CV scripts for camera input
* SLAM & path planning using LiDAR data
* Autonomous navigation (in planning phase)

## Documentation

Please see `JOURNAL.md` for daily progress, planning, and development logs.

## Licensing

MIT License for once.

---
