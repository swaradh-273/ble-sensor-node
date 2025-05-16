# BLE Sensor Node – ESP32-C3 + BME280

## 🧠 Overview
This project simulates a low-power BLE sensor node using the ESP32-C3 and BME280 environmental sensor. The node is designed for wireless data transmission over BLE, with onboard voltage regulation and I²C communication between components.

## 🔧 Project Scope
- Simulated using EasyEDA (schematic + layout)
- Designed for low-power applications (battery-powered)
- Environmental sensing via BME280 (temperature, humidity, pressure)
- BLE transmission using ESP32-C3 onboard radio
- Regulated via MCP1700 3.3V LDO for sensor stability

## 🖼️ Schematic
![BLE Schematic](https://github.com/swaradh-273/ble-sensor-node/blob/main/images/ble_schematic.png?raw=true)


## ⚙️ Components
- ESP32-C3 (BLE + Wi-Fi capable microcontroller)
- BME280 Sensor (I²C)
- MCP1700 3.3V LDO
- Pull-up resistors for I²C lines
- Diode protection and power input filtering

## 🚫 Note
This project is **simulation only** and was not physically assembled or tested. PCB and circuit design were completed and verified using EasyEDA’s simulation and validation tools.

## 📎 Project Files
- Schematic (`.png`)

