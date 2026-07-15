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
- Responsive and intuitive control scheme

## Installation

### Prerequisites

- ev3dev installed on your EV3 brick
- Python 3 with pybricks library

### Setup

1. Clone or download this repository to your EV3 device
   ```bash
   git clone https://github.com/ceyale/PS4-Controller-ev3.git
   ```

2. Transfer `ps4controller_ev3dev/main.py` to your EV3 brick

3. Connect your PS4 controller to the EV3 device via Bluetooth

### Running the Program

Execute the script using pybricks-micropython:

```bash
pybricks-micropython main.py
```

## Controls

- **Right Analog Stick**:
  - **Up/Down (Y-axis)**: Control forward/backward movement
  - **Left/Right (X-axis)**: Control steering

## Project Structure

```
PS4-Controller-ev3/
├── README.md                    # This file
├── ps4controller_ev3dev/
│   └── main.py                  # Main control script
└── [other source files]
```

## How It Works

The script reads input from the PS4 controller's analog sticks and translates them into motor speed commands for the EV3:
- The Y-axis of the right stick controls forward/backward motion
- The X-axis controls steering by adjusting motor speeds differentially
- Motor speeds are scaled smoothly from -100 (reverse) to 100 (forward)

## Troubleshooting

- **Controller not connecting**: Ensure PS4 controller is in pairing mode and properly paired via Bluetooth
- **Motors not responding**: Verify motors are connected to ports B and C on the EV3 brick
- **Script errors**: Check that pybricks library is properly installed on your EV3 device

## Requirements

See `requirements.txt` for Python dependencies.

## Contributing

Contributions are welcome! Feel free to:
- Report bugs and issues
- Suggest new features
- Submit pull requests with improvements

## License

[Specify your license here]

## Resources

- [ev3dev Documentation](https://www.ev3dev.org/)
- [PyBricks Documentation](https://pybricks.com/)
- [LEGO Mindstorms EV3](https://www.lego.com/en-us/themes/mindstorms)
- [PS4 Controller Information](https://www.playstation.com/en-us/accessories/dualshock-4-wireless-controller/)

## Author

ceyale

---

**Note**: This project is designed for educational and hobbyist purposes. Always ensure your robot is operated in a safe environment.
