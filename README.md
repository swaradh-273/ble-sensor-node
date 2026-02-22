# ESP32 BLE Environmental Sensor Node

This project implements a low-power environmental monitoring node using the ESP32 and BME280 sensor. The ESP32 communicates with the BME280 over I²C to read temperature and humidity data, then broadcasts the readings wirelessly using Bluetooth Low Energy (BLE).

The system includes proper power regulation, I²C pull-up configuration, boot/reset circuitry, and antenna clearance considerations for reliable wireless performance. All hardware was first prototyped and then designed for PCB implementation.

This project demonstrates embedded system design fundamentals including power management, sensor interfacing, BLE communication, and hardware layout practices.

# Hardware Description

This project is based on the ESP32-C3-WROOM-02 module integrated with a BME280 environmental sensor. The ESP32 operates at 3.3V, powered through an onboard LDO voltage regulator with proper input/output decoupling capacitors for stable operation.

The BME280 is interfaced using the I²C protocol (SDA and SCL lines) with external pull-up resistors to 3.3V. CSB is tied high to enable I²C mode, and SDO is grounded to select the 0x76 I²C address. A 100nF decoupling capacitor is placed close to the sensor supply pins for noise suppression.

The ESP32 boot and enable pins are configured using 10k pull-up resistors and push-button switches for manual reset and flash mode selection. A 4-pin UART header (3V3, GND, TX, RX) is provided for programming and debugging.

Special care is taken to maintain antenna clearance by keeping copper and ground planes away from the PCB antenna region to ensure reliable BLE performance.

## 🖼️ Schematic
images/SCH_Schematic1_1-P1_2026-02-22.png



## 📎 Project Files
- Schematic (`.png`)

