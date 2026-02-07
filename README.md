# Embedded Sentry System

## Overview
Gesture-based security system on the STM32F429i Discovery (ARM Cortex-M4). Uses gyroscope data to recognize predefined motion patterns for system access control. Built with PlatformIO.

## Features

- Real-time gyroscope data capture and processing (L3GD20 sensor)
- Gesture recognition for system access control
- LCD display output (ILI9341) and touch screen interface (STMPE811)
- Serial data logging for analysis and debugging
- Configurable gesture thresholds and calibration

## Project Structure
The project consists of the following key components:

- `gyro.h` / `gyro.cpp`: Core gyroscope functionality implementation including data capture and processing
- `serial_dump.py`: Python-based debugging tool for raw sensor data analysis
- `system_config.h`: Central configuration file containing system parameters and constants
- `utilities.h` / `utilities.cpp`: Common utility functions for data processing and system management

## Installation

### Prerequisites
Before installing, ensure you have:

- C++ compiler (GCC or Clang)
- Python installation
- Serial communication tool (Arduino IDE or minicom)

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/XhovaniM8/embedded-sentry.git
   cd embedded-sentry
   ```

2. Open the project:
   - Launch Visual Studio Code
   - Ensure PlatformIO extension is installed
   - Open the project folder

3. Build the project:
   - Press `Ctrl + Shift + P` (Windows/Linux) or `Cmd + Shift + P` (macOS)
   - Select "PlatformIO: Build"

4. Upload to device:
   ```bash
   pio run --target upload
   ```

## Configuration

The `system_config.h` file contains essential system parameters:

- Gesture recognition threshold values
- Gyroscope calibration settings
- System timing parameters

Modify these settings to optimize system performance for your specific use case.

## Contributing

We welcome community contributions to enhance the Embedded Sentry System. To contribute:

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Submit a pull request

### Development Team

- Xhovani Mali (xxm202) - Developer
- Temira Koenig (trk8600) - Developer
- Shruti Tulshidas Pangare - Developer

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for complete details.
