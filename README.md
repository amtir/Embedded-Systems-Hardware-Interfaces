# Embedded Systems & Hardware Interfaces

A portfolio of embedded and IoT projects from 2010 to 2022: sensor drivers, industrial bus protocols, cellular connectivity, microcontroller firmware and desktop tools that talk to hardware. Each project is its own repository, linked here as a **git submodule** and grouped by domain.

## Projects

### 🔌 Sensors

| Project | Interface | Description |
|---------|-----------|-------------|
| [TOF Proximity Sensors](https://github.com/amtir/TOF_Sensors_UART_Cascade) | UART | 5 laser Time-of-Flight range sensors chained on one UART bus; binary frame decoding with checksum |
| [Ultrasonic Distance Sensors](https://github.com/amtir/Ultrasonic_Distance_Sensors) | GPIO | 8 × HC-SR04 sensors triggered in sequence, with a watchdog timeout |
| [Gesture Recognition Sensors](https://github.com/amtir/Multiplexing_Gesture_Recognition_Sensors_I2C) | I²C | 8 × PAJ7620U2 sensors that share one I²C address, behind a TCA9548A multiplexer |
| [Liquid Level Sensor](https://github.com/amtir/Liquid_Level_Detection) | GPIO | GEMS ELS-950 electro-optic level switches, debounced and logged to CSV with plots |
| [Temperature DS18B20](https://github.com/amtir/Temperature_DS18B20_Python) | 1-Wire | Four DS18B20 sensors on one bus, with rotating-file logging |
| [1-Wire iButton](https://github.com/amtir/1Wire_iButton) | 1-Wire | Dallas iButton reader for identification and access control |
| [RFID / NFC](https://github.com/amtir/RFID_NFC_NXP_PN512_Python) | SPI | NXP PN512 (EXPLORE-NFC) MIFARE / NFC tag reader |

### 📈 Analog-to-Digital Converters

| Project | Interface | Description |
|---------|-----------|-------------|
| [MCP3424 18-bit ADC](https://github.com/amtir/MCP3424_ADC_18bits_PGA) | I²C | Two MCP3424 ADCs measuring NTC temperature (Steinhart–Hart), pressure and power, with calibration |

### 📡 IoT Connectivity

| Project | Technology | Description |
|---------|------------|-------------|
| [NB-IoT SIM7000](https://github.com/amtir/QoS_NB-IoT_SIM7000) | NB-IoT / LTE-M | Signal-quality monitor with a PyQt5 GUI, UDP/HTTP telemetry and GPIO power control |
| [SMS Parser](https://github.com/amtir/sms_parser) | 4G LTE | Remote device commands sent by SMS, through the Huawei E3372 HiLink API |
| [NanoPi IoT Gateway](https://github.com/amtir/NanoPi_IoT_Gateway) | UART / Ethernet | Evaluation of the NanoPi NEO2 as a serial-to-network gateway |
| [RTC Synchronization](https://github.com/amtir/RTC_Network_Time_Synchronization) | NTP | Forces a clock resync on IoT devices as soon as they are online |

### 🌬️ Weather Station

| Project | Platform | Description |
|---------|----------|-------------|
| [NMEA LCD Display](https://github.com/amtir/NMEA_LCD_DISPLAY) | 8051 (C) | Standalone RS-485 NMEA 0183 display: firmware, OrCAD schematic, enclosure |
| [PC Weather Display](https://github.com/amtir/PC_program_NET_Display_NMEA) | VB.NET | Windows app with live values, real-time charts and an installer |

### 🚗 Automotive

| Project | Platform | Description |
|---------|----------|-------------|
| [OBD-II Diagnostic GUI](https://github.com/amtir/OBDII_PC_Program_GUI) | VB.NET | ELM327 scan-tool client: live engine data, data logger, trouble codes |

## Skills Demonstrated

- **Buses & protocols**: I²C (with multiplexing), SPI, UART / RS-232 / RS-485, 1-Wire, NMEA 0183, OBD-II, AT commands
- **Connectivity**: NB-IoT, LTE / 4G, 3G, PPP, UDP, HTTP, NTP
- **Platforms**: Raspberry Pi, NanoPi, 8051 microcontrollers, Windows desktop
- **Languages**: Python, C, VB.NET, Bash
- **Engineering**: signal conditioning and sensor calibration, debouncing, watchdogs, schematic capture (OrCAD), enclosure and power design

## Cloning

```bash
# Everything, including all project submodules
git clone --recurse-submodules https://github.com/amtir/Embedded-Systems-Hardware-Interfaces.git

# Update every submodule to the latest version of its project
git submodule update --remote --merge
```

## Author

**Akram M'Tir**, Software Engineer & Solution Architect, [@amtir](https://github.com/amtir)
