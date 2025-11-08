# MCU Data Logger with Memory and Clock

This project is a **microcontroller-based data logger** that integrates a Real-Time Clock (RTC) and external EEPROM memory. It is designed to collect sensor or system data and store it with accurate timestamps for future analysis.

## Features

- **ATmega328P-AU** microcontroller (TQFP package)
- **DS1337S+ Real-Time Clock** with 32.768kHz crystal for precise timestamping
- **Two 24LC1025 EEPROMs** (I2C) for 256 KB non-volatile memory
- ISP programming and UART debugging headers
- Status LEDs and reset circuitry
- **PCB layout: 4-layer** (optimized for signal integrity and EMI performance)

## Technical Highlights

| Component     | Description                              |
|---------------|------------------------------------------|
| MCU           | ATmega328P-AU (TQFP-32)                  |
| RTC           | DS1337S+ with external 32.768kHz crystal |
| Memory        | 2x 24LC1025 EEPROM (via I2C)             |
| Interfaces    | I2C, UART, SPI (for flashing/debug)      |
| Supply        | External power input with decoupling     |
| Mounting      | 4x Mounting holes for enclosure          |
| PCB Versions  | 2-layer and 4-layer available            |

## Schematic

![Schematic](/schmatics.png)

## PCB Versions

- **4-Layer Version**: Includes dedicated power and ground planes for improved performance and reduced noise in analog/digital domains.

  ![PCB](/pcb(2).png)

## Notes

- The design is **based on guided tutorials** and **open-source references**, but modified for personal understanding and improvement.
- EEPROM addresses and pull-up resistors are configured for standard I2C communication.
- RTC supports battery backup for long-term timekeeping even when power is lost.

## License

This project is licensed under the *** License – feel free to build, modify, and share!

*(Design created using KiCad 8.0.9)*
