# PS4 Controller EV3

Control your LEGO EV3 robot using a PlayStation 4 controller!

## Overview

This Python project enables wireless control of an EV3 robot using a PS4 controller. It bridges the gap between gaming peripherals and robotics, making robot operation intuitive and fun.

## Features

- 🎮 **PS4 Controller Support** - Use your PlayStation 4 controller to command the EV3
- 🤖 **EV3 Robot Control** - Full motor and sensor integration
- ⚡ **Real-time Response** - Low-latency input processing
- 🔌 **Wireless Operation** - Control your robot over Bluetooth
- 🎯 **Intuitive Controls** - Tank-style drive mapping for precise movement

## Requirements

- Python 3.x
- LEGO EV3 Mindstorms brick running ev3dev
- PlayStation 4 controller (DualShock 4)
- EV3 robotics libraries (pybricks or ev3dev)
- PS4 controller library support

## Installation

1. Clone this repository:
```bash
git clone https://github.com/ceyale/PS4-Controller-ev3.git
cd PS4-Controller-ev3
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

3. Transfer the scripts to your EV3 device

4. Ensure your EV3 is connected and running ev3dev firmware

5. Pair your PS4 controller via Bluetooth to the EV3

## Usage

Run the main script to start controlling your EV3:

```bash
pybricks-micropython main.py
```

### Controller Mapping

| Input | Action |
|-------|--------|
| Right Stick Y-Axis | Forward/Backward Movement |
| Right Stick X-Axis | Left/Right Steering |
| Motor Ports B & C | Left and Right Drive Motors |

## Project Structure

```
PS4-Controller-ev3/
├── README.md                      # Documentation
├── requirements.txt               # Python dependencies
├── ps4controller_ev3dev/
│   └── main.py                    # Main control script
└── [additional files]
```

## Hardware Setup

- **EV3 Brick**: Running ev3dev operating system
- **Motors**:
  - Port B: Left motor
  - Port C: Right motor
- **Controller**: PS4 DualShock 4 via Bluetooth connection

## How It Works

The script reads input from the PS4 controller's analog sticks and translates them into motor speed commands:

1. **Y-Axis (Forward/Backward)**: Controls the base movement speed (-100 to 100)
2. **X-Axis (Steering)**: Adjusts motor speeds differentially for turning
3. **Differential Speed**: Calculates individual motor speeds for smooth tank-style turns
4. **Motor Output**: Commands sent to motors on ports B and C

## Troubleshooting

| Issue | Solution |
|-------|----------|
| Controller not detected | Ensure PS4 controller is properly paired via Bluetooth |
| EV3 not responding | Verify ev3dev firmware is installed and up-to-date |
| Motors not moving | Check motor connections to ports B and C |
| Permission errors | May require elevated privileges for controller access on Linux |
| Script errors | Verify pybricks library is installed on the EV3 device |

## Configuration

Edit `main.py` to customize:
- Motor ports and speeds
- Controller sensitivity
- Drive control scheme
- Response thresholds

## Contributing

Contributions are welcome! To contribute:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is provided as-is for educational and hobbyist purposes.

## Resources

- [ev3dev Documentation](https://www.ev3dev.org/)
- [PyBricks Documentation](https://pybricks.com/)
- [LEGO Mindstorms EV3](https://www.lego.com/en-us/themes/mindstorms)
- [PlayStation 4 Controller](https://www.playstation.com/en-us/accessories/dualshock-4-wireless-controller/)

## Safety Notice

⚠️ **Important**: Always operate your robot in a safe, controlled environment away from obstacles and people. Ensure proper supervision during testing and operation.

## Author

ceyale

---

**Enjoy controlling your EV3 with your PS4 controller!** 🚀
