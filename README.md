
# DC Motor Speed Control using STM32

## Project Overview

This project implements a DC motor speed control system using an STM32 microcontroller.

The system uses PWM to control motor speed, an encoder to measure actual motor speed, and a PID controller to regulate the motor based on feedback.

The motor speed and system status are displayed on an LCD, while UART communication is used to monitor system information through a virtual terminal.

## Features

- PWM-based DC motor speed control.
- Encoder feedback for motor speed measurement.
- PID control for speed regulation.
- LCD display for real-time speed monitoring.
- UART communication for debugging and monitoring.
- Real-time motor speed adjustment.

## Hardware Components

- STM32F103C8T6 Microcontroller
- DC Motor with Encoder
- L298 Motor Driver
- LCD 16x2
- Virtual Terminal
- Power Supply

## STM32 Peripherals

| Peripheral | Function |
|---|---|
| TIM1 - PWM | Generates PWM signals to control motor speed |
| TIM3 - Encoder Mode | Reads encoder signals to measure motor speed |
| USART1 | Transmits monitoring data to the virtual terminal |
| GPIO | Controls peripheral interfaces |
| GPIO LCD Interface | Sends commands and data to the LCD |

## System Operation

1. The STM32 initializes the system peripherals.
2. PWM signals are generated to control the motor.
3. The encoder provides feedback about motor rotation.
4. The STM32 calculates the actual motor speed.
5. The PID controller processes the speed error and adjusts the PWM output.
6. The LCD displays the motor speed.
7. UART transmits system information for monitoring.

## Simulation Results

The system was designed and tested using Proteus simulation.

The main functions include:

- **Motor Startup:** Initializes the motor control system.
- **PWM Speed Control:** Adjusts the PWM duty cycle to control motor speed.
- **Encoder Feedback:** Uses encoder signals to calculate actual motor speed.
- **PID Speed Regulation:** Adjusts PWM output based on the difference between target and actual speed.
- **LCD Monitoring:** Displays motor speed and system information.
- **UART Monitoring:** Transmits system data through the virtual terminal.

## Project Structure

```text
DC-Motor-Speed-Control-STM32/
│
├── Core/
│   ├── Inc/
│   └── Src/
│
├── Drivers/
│
├── Proteus/
│
├── README.md
└── ...
```

## How to Run

### 1. Open the STM32 Project

- Open STM32CubeIDE.
- Import the project into the workspace.
- Build the project to compile the source code.

### 2. Run the Proteus Simulation

- Open the Proteus project file.
- Configure the STM32 microcontroller with the compiled HEX file if required.
- Start the simulation.
- Observe motor operation, LCD display, and virtual terminal.

### 3. Monitor System Performance

- Observe motor speed changes.
- Monitor encoder feedback.
- Check PID speed regulation.
- View UART data through the virtual terminal.

## Technologies Used

- C Programming
- STM32 Microcontroller
- STM32CubeIDE
- Proteus Design Suite
- PWM
- Encoder Interface
- PID Control
- UART Communication

## Author

**Ngo Phuc Huy**

Fourth-year Microelectronics Engineering Student

GitHub: [huycorn1003](https://github.com/huycorn1003)
