# Smart-Industrial-Temperature-Monitoring-MCU-Board
Smart Industrial Temperature Monitoring MCU Board is a 24V IoT-based development board designed for industrial applications. It monitors machine temperature and detects overheating conditions. The board supports Wi-Fi alerts, EEPROM data logging, and optocoupler isolation for reliable operation.
Smart-Industrial-Temperature-Monitoring-MCU-Board
Smart Industrial Temperature Monitoring MCU Board is a 24V IoT-based development board designed for industrial applications. It monitors machine temperature and detects overheating conditions. The board supports Wi-Fi alerts, EEPROM data logging, and optocoupler isolation for reliable operation. Smart health monitoring and predective monitoring system

Abstract

The Smart Industrial Machine Health and Predictive Monitoring System is an embedded IoT-based industrial monitoring platform designed using the PIC16F877A microcontroller. The system integrates power protection, sensing, control, and wireless communication modules to ensure real-time machine condition monitoring, fault detection, and predictive maintenance capability. The design emphasizes industrial safety, reliability, and remote accessibility through Wi-Fi connectivity.

System Architecture

🔌 Power Distribution Flow 24 V DC Input ↓ PTC Resettable Fuse (Overcurrent Protection) ↓ TVS Diode (Surge Protection) ↓ Reverse Polarity Protection Diode ↓ LM2596-5.0 Buck Converter (24 V → 5 V) ↓ 5 V Power Rail → MCU, Sensors, EEPROM ↓ 3.3 V Regulator → ESP8266 Wi-Fi Module

INPUT MODULES

Power Input Interfaces DC Barrel Jack (24 V input) USB 2.0 Port (5 V interface) 2-Pin Power Header (external supply)
PROTECTION CIRCUITRY Overcurrent Protection PTC Resettable Fuse (750 mA) Protects against short circuit and overload Surge Protection TVS Diode (33 V) Clamps voltage spikes and transient surges Reverse Polarity Protection Schottky diode blocks wrong polarity connection

POWER SUPPLY UNIT LM2596-5.0 Buck Converter (24 V → 5 V) 680 µF input filtering capacitor 33 µH inductor (energy storage element) 220 µF output capacitor (ripple reduction)

CONTROL UNIT PIC16F877A Microcontroller (Main controller) 16 MHz Crystal Oscillator (clock source) 22 pF load capacitors 100 nF decoupling capacitor MCLR reset circuit External EEPROM (data storage)

COMMUNICATION MODULE ESP-01M (ESP8266 Wi-Fi Module) UART TX/RX communication 3.3 V supply via regulator IoT-based wireless monitoring

SENSING UNIT LM35DZ temperature sensor Real-time machine temperature monitoring Fault detection based on overheating

ISOLATION CIRCUIT PC817 Optocoupler Provides electrical isolation Protects microcontroller from high voltage noise

OUTPUT SECTION Buzzer (alarm system via transistor driver) 3 Red LED indicators Power / Status / Fault indication

SCHEMATIC

<img width="872" height="575" alt="image" src="https://github.com/user-attachments/assets/8a8495e6-c70a-4fe5-827a-39bba7900b49" />
<img width="1161" height="650" alt="image" src="https://github.com/user-attachments/assets/3837365e-1a03-4d85-8364-b86f73d2cc6d" />

LAYOUT

<img width="502" height="318" alt="image" src="https://github.com/user-attachments/assets/7a22e084-47fc-4bde-9c91-c4a41b1cefc4" />
<img width="506" height="323" alt="image" src="https://github.com/user-attachments/assets/4ab6f0b6-d4f4-4759-b595-7b79d927fbe7" />


3D MODEL

<img width="486" height="320" alt="image" src="https://github.com/user-attachments/assets/9d5ff4f2-93d9-4a3a-88bb-31659ecc5e3d" />
<img width="1048" height="601" alt="Screenshot 2026-06-24 085353" src="https://github.com/user-attachments/assets/09f90a2b-4d17-45f3-957d-bdb3bb883250" />


FEATURES Multi-level protection (PTC + TVS + reverse polarity) Wi-Fi based IoT monitoring (ESP8266) Real-time temperature monitoring (LM35) Electrical isolation for safety (PC817) Non-volatile data storage (EEPROM)
