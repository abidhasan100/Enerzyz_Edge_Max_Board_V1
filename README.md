# Enerzyz_Edge_Max_Board_V1

## Overview

This project is based on the **Luckfox Pico Plus** development board. The repository contains source code, setup instructions, hardware connections, and deployment steps for building and running the project.


## Board Information

### Hardware

* Board: Luckfox Pico Plus
* Processor: Rockchip RV1103
* Architecture: ARM Cortex-A7
* Connectivity: USB, GPIO, UART, SPI, I2C
* Operating System: Linux

### Features

* Compact embedded Linux platform
* GPIO control support
* UART communication
* SPI and I2C peripheral support
* Camera interface support
* Lightweight and power-efficient


## Project Structure

```bash
.
├── src/                # Source code
├── scripts/            # Utility scripts
├── docs/               # Documentation
├── build/              # Build output
├── firmware/           # Firmware files
├── images/             # Images and screenshots
├── README.md           # Project documentation
└── LICENSE             # License file
```


## Requirements

### Hardware Requirements

* Luckfox Pico Plus board
* USB Type-C cable
* MicroSD card (if required)
* Power supply
* Ethernet/WiFi connection (optional)

### Software Requirements

* Linux / Windows / macOS
* Git
* SSH client
* Cross compiler toolchain (optional)
* Python 3.x (if required)


## Installation

### Clone the Repository

```bash
git clone https://github.com/abidhasan100/Enerzyz_Edge_Max_Board_V1.git
cd Enerzyz_Edge_Max_Board_V1
```

### Build the Project

```bash
mkdir build
cd build
cmake ..
make
```

## Flashing Firmware

### Enter Loader Mode

1. Connect the board via USB.
2. Hold the BOOT button.
3. Power on the board.
4. Release the button after detection.

### Flash the Image

```bash
sudo upgrade_tool di firmware/update.img
```


## Running the Project

### Start Application

```bash
./your_application
```

### Run Python Script

```bash
python3 main.py
```


## GPIO Example

### Export GPIO

```bash
echo 23 > /sys/class/gpio/export
```

### Set Direction

```bash
echo out > /sys/class/gpio/gpio23/direction
```

### Turn GPIO ON

```bash
echo 1 > /sys/class/gpio/gpio23/value
```

### Turn GPIO OFF

```bash
echo 0 > /sys/class/gpio/gpio23/value
```

## UART Example

### Open Serial Console

```bash
screen /dev/ttyUSB0 115200
```


## SSH Access

### Connect via SSH

```bash
ssh root@192.168.1.100
```

## Troubleshooting

### Device Not Detected

* Check USB cable quality
* Verify drivers are installed
* Reboot the board

### Flashing Failed

* Ensure loader mode is active
* Use correct firmware image
* Try another USB port

### Permission Issues

```bash
sudo chmod +x your_application
```


## Screenshots

Add project screenshots inside the `images/` folder.

Example:

```markdown
![Project Screenshot](images/project.png)
```


## Future Improvements

* Add web dashboard
* Add OTA update support
* Improve power optimization
* Add MQTT support
* Add sensor integrations


## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.


## License

This project is licensed under the ENERZYZ Limited License.


## Author

**Mir Md Abid Hasan**

* GitHub: [https://github.com/abidhasan100](https://github.com/abidhasan100)
* Repository: [https://github.com/abidhasan100/Enerzyz_Edge_Max_Board_V1](https://github.com/abidhasan100/Enerzyz_Edge_Max_Board_V1)
