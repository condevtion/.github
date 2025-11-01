# Condevtion

## About

Within these pages, the arcane code and whispered secrets of the I2C Sensors board are now unveiled. We invite the curious to delve into its digital heart.

## The Triple Eye of Observation: I2C Sensors Board

A nexus of three little digital sensors - each a tiny sentinel gathering data from the ether. They measure the very breath of the air - pressure, the mists and fever of the surroundings - relative humidity and temperature, and the hidden spectrum and the Glow - light and color.

<img width="320" height="290" alt="I2CSensors Board" src="https://github.com/user-attachments/assets/269caf3b-be8b-4e8b-b98a-6cf10cff9b34" />

All three miniature eyes draw their strength from a common 3.3V power stream (`VDD`, `GND`), and commune via the sacred I2C bus (`SCL`, `SCA`). This bus is fortified with pull-up resistors, ensuring the messages are not lost to the void. For those requiring immediate, urgent notifications, the interrupt lines for the pressure and ambient light sensors (`IP`, `IL`) stand exposed and ready to signal.

Assembled samples are available at ebay - [Temperature, Pressure, Humidity, Light, and Color I2C Sensors Board](https://ebay.us/m/AJYYwf).

## The Breath of the Air: Pressure

The SPL07-003 a miniaturized digital barometric air pressure sensor from [Goermicro](https://en.goermicro.com/) (U1) is the component responsible for sensing the great weight of the atmosphere. Its I2C calling address can be mystically altered by the solder jumper (J3). For deeper study into its workings, consult its ancient scroll [SPL07-003.pdf](https://media.digikey.com/pdf/Data%20Sheets/Goertek%20Microelectronics%20PDFs/SPL07-003.pdf) in DigiKey's scriptorium.

## The Mists and the Fever: Humidity and Temperature

For divining the environment's relative humidity and its precise temperature, we rely on the ENS210 sensor from [ScioSense](https://www.sciosense.com/). This clever chip is a dual-purpose artifact, featuring both a humidity detector and a surprisingly accurate thermometer. The full spellbook is detailed in the [ENS210-Datasheet.pdf](https://www.sciosense.com/wp-content/uploads/2025/09/ENS210-Datasheet.pdf).

## The Hidden Spectrum and the Glow: Ambient Light and Color

The APDS-9999 from [Broadcom](https://www.broadcom.com/) is the eye that sees beyond. It measures ambient light, the invisible infrared, and the glorious RGB hues. It is the keeper of the colors and the light's intensity. Unlock its secrets on its own illuminated page - [APDS-9999](https://www.broadcom.com/products/optical-sensors/integrated-ambient-light-and-proximity-sensors/apds-9999).

## The Vision of the Aether: Tools
Should you seek to capture the raw whispers of the sensors, the [i2cs-test](https://github.com/condevtion/i2cs-test) utility is your initial scrying pool. Though meant for trials, it can fully extract all data from the I2C sensors. Once these secrets are bound, the powerful [i2cs-graph](https://github.com/condevtion/i2cs-graph) utility is summoned. This potent spell transforms the raw whispers into magnificent charts and spectral lines, allowing the initiated to gaze upon the flow of data.

<img width="651" height="509" alt="I2CS-data" src="https://github.com/user-attachments/assets/038d8b69-3c94-4f1b-be64-43c09d959b49" />
