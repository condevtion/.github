# Condevtion

## About

Condeviton is the home for the I2C Sensors Board, offering open-source schematics and code for a compact sensor platform.

## I2C Sensors Board

The board features a set of three miniature digital sensors. They measure temperature, pressure, relative humidity, ambient light and color (RGB).

<img width="320" height="290" alt="I2CSensors Board" src="https://github.com/user-attachments/assets/269caf3b-be8b-4e8b-b98a-6cf10cff9b34" />

All the sensors powered from a common 3.3V source (`VDD`, `GND`), and communicate over I2C bus (`SCL`, `SCA`) which is already equipped with pull-up resistors. Additionally, pressure and light sensor's interrupt lines exposed on dedicated pins (`IP`, `IL`).

Assembled samples are available at ebay - [Temperature, Pressure, Humidity, Light, and Color I2C Sensors Board](https://ebay.us/m/AJYYwf).

## Pressure

SPL07-003 is responsible for air pressure measurements. It is a miniaturized digital barometric sensor from [Goermicro](https://en.goermicro.com/) (U1). Its I2C address can be altered by the solder jumper (J3). For mor details consult its datasheet [SPL07-003.pdf](https://media.digikey.com/pdf/Data%20Sheets/Goertek%20Microelectronics%20PDFs/SPL07-003.pdf) in DigiKey's media storage.

## Humidity and Temperature

For relative humidity and temperature measurements the board relies on the ENS210 sensor from [ScioSense](https://www.sciosense.com/). The chip contains high accuracy temperature sensor (0.15°C). More information can be found in the [ENS210-Datasheet.pdf](https://www.sciosense.com/wp-content/uploads/2025/09/ENS210-Datasheet.pdf).

## Ambient Light and Color

The APDS-9999 from [Broadcom](https://www.broadcom.com/) is an ambient light, infrared, and RGB sensor. It can be configured to measure overall illuminance or to use four individual channels for red, green, blue, and infrared light. See further description on its page - [APDS-9999](https://www.broadcom.com/products/optical-sensors/integrated-ambient-light-and-proximity-sensors/apds-9999).

## Tools

The board can be tested and simple measurements can be done with [i2cs-test](https://github.com/condevtion/i2cs-test) utility. Data gathered by it can be visualized by [i2cs-graph](https://github.com/condevtion/i2cs-graph). It produces charts for main measured values - temperature, pressure, relative humidity, illuminance, relative infrared readings, normalized RGB channels, and shows measured colors as RGB chart background.

<img width="651" height="509" alt="I2CS-data" src="https://github.com/user-attachments/assets/038d8b69-3c94-4f1b-be64-43c09d959b49" />
