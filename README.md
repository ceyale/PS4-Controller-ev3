# PS4 Controller EV3

Control an EV3 robot with a PlayStation 4 controller.

## Overview

This project enables you to control a LEGO EV3 robot with two motors using a PS4 controller connected to an EV3 device running ev3dev.

## Hardware Requirements

- **LEGO EV3 Brick** running ev3dev
- **PS4 Controller** (DualShock 4)
- **Two Motors** connected to the EV3:
  - Left motor: Port B
  - Right motor: Port C

## Features

- Real-time motor control using PS4 controller analog sticks
- Smooth motor speed scaling (-100 to 100)
- Tank-style drive control using right analog stick:
  - **Y-axis**: Forward/Backward movement
  - **X-axis**: Left/Right steering
- Differential speed calculation for turning

## Installation

### Prerequisites

- ev3dev installed on your EV3 brick
- Python 3 with pybricks library

### Setup

1. Clone or download this repository to your EV3 device
2. Transfer `ps4controller_ev3dev/main.py` to your EV3 brick
3. Connect your PS4 controller to the EV3 device via Bluetooth

### Running the Program

Execute the script using pybricks-micropython:

```bash
pybricks-micropython main.py
