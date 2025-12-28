# LED Cube Firmware System

## Overview
This project implements a real-time embedded software system to control an 8×8×8 LED cube using multiplexing and precise timing constraints. The firmware is written in C++ and designed to operate reliably on resource-constrained microcontroller hardware.

## Key Features
- Real-time multiplexed LED control with deterministic refresh timing
- Efficient memory usage for 512-addressable LEDs
- Stable refresh behavior under strict timing constraints
- Modular firmware structure for readability and extensibility

## Technical Details
- Language: C++
- Architecture: Timer-driven control loop with multiplexed addressing
- Constraints: Limited memory, strict refresh timing, real-time stability
- Debugging: Identified and resolved refresh-rate instability through systematic testing

## Challenges & Solutions
One of the primary challenges was eliminating flicker caused by timing drift during LED refresh cycles. This was resolved by restructuring the control loop and optimizing timing logic to ensure consistent refresh intervals.

## What I Learned
- Designing software under real-time constraints
- Debugging timing-related failures in embedded systems
- Writing maintainable, low-level C++ for hardware interaction
- Translating system behavior into deterministic software logic

## Future Improvements
- Add pattern scripting support
- Improve animation abstraction layer
- Port firmware to additional microcontroller platforms
