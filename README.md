# weather-balloon-hat
A small Raspberry Pi Hat as basis for a weather balloon payload

# Features

  * Connectors for 6 Grove I2C and 2 Grove digital IO
  * Ublox GPS module
  * LoRa Transceiver
  * Configuable hardware watchdog
  * Wide range Step-Up/Step-Down DC/DC as power supply
  * Selectable I/O voltage (3.3V/5V)
  * Screw holes for Raspberry Pi B and Zero

# Schematic

[schematic](schematic/Schematic_Weatherballoon-Hat_v0.6.pdf)

# Watchdog

Maxim MAX6369KA+T

[datasheet](https://datasheets.maximintegrated.com/en/ds/MAX6369-MAX6374.pdf)


# LoRa

HopeRF RFM95

# GPS

Ublox CAM-M8Q

# Power

Pololu 5V Step-Up/Step-Down Voltage Regulator S18V20F5

[link](https://www.pololu.com/product/2574)

# IO


## Pinout

| Pin | BCM | Function | Used for |
| --: | --: | -------- | -------- |
| 3   |  2  | SDA      | I2C      |
| 5   | 3   | SCL      | I2C      |
| 7   | 4   | GPIO     | opt. WittyPi |
| 11  | 17  | GPIO     | opt. WittyPi |
| 13  | 27  | GPIO     | RFM95 DIO0 |
| 15  | 22  | GPIO     | Grove digital J2 |
| 19  | 10  | MOSI     | RFM95 SPI |
| 21  | 9   | MISO     | RFM95 SPI |
| 23  | 11  | SCK      | RFM95 SPI |
| 29  | 5   | GPIO     | RFM95 DIO1 |
| 31  | 6   | GPIO     | RFM95 DIO2 |
| 33  | 13  | Out      | RFM95 Reset |
| 35  | 19  | Out      | Watchdog cycle SET1|
| 37  | 26  | Out      | Watchdog cycle SET0|
|   8 | 14  | TXD      | GPS TX |
| 10  | 15  | RXD      | GPS RX |
| 12  | 18  | IN       | GPS PPS |
| 16  | 23  | GPIO     | Grove digital J2 |
| 18  | 24  | GPIO     | Grove digital J1 |
| 22  | 25  | GPIO     | Grove digital J1 |
| 24  | 8   | CE0      | RFM95 SPI |
| 26  | 7   | IN       | GPS Interupt |
| 32  | 12  | Out      | GPS Reset |
| 36  | 16  | Out      | Watchdog heartbeat |
| 38  | 20  | Out      | LED0 |
| 40  | 21  | Out      | LED1 |
