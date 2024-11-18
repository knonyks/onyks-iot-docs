# ONYKS IoT - Documentation

## 18.11.2024

### What we use

- Module [ESP32-WROOM-32D](https://www.espressif.com/sites/default/files/documentation/esp32-wroom-32d_esp32-wroom-32u_datasheet_en.pdf)
- Program [KiCAD](https://www.kicad.org/) version 8
- GitHub for project storage

### Tasks for the next meeting

- Consider how the device should work
- Find the main peripherals meeting the project requirements
- Plan the maximum current consumption for the selected peripherals
  - Do not design the power supply circuit yet
- Optional: create a small diagram in [drawio](https://app.diagrams.net/)
- Familiarize yourself with the example devboard

### Where to read

- Official [devboard](https://docs.espressif.com/projects/esp-dev-kits/en/latest/esp32/esp32-devkitc/user_guide.html) - worth reviewing
  - Documentation at the bottom: technical specification, schematics, PCB
- Introduction to [KiCAD](https://docs.kicad.org/8.0/en/getting_started_in_kicad/getting_started_in_kicad.html)
- For the future, you can read in your free time [Introduction to ESP32](https://docs.espressif.com/projects/esp-idf/en/v5.3.1/esp32/get-started/index.html)

### Basic assumptions

- Power supply: 3.3 V
- Bluetooth communication (at this stage, just a curiosity)
- No programmer on the board (programmers will be separate)
- UART and JTAG interfaces for programming and debugging
- "Reset" button
