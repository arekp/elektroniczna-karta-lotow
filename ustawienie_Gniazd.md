# SPI #

| Nazwy | Nokia (numer goldpina) | SD card (numer goldpina) |NR Gniazda |
|:------|:-----------------------|:-------------------------|:----------|
|DIN-DI-MISO |4 | 2 | 11 |
|DC-DO-MOSI | 3 | 4 | 12 |
|CLK-CLK-SCK | 5 | 3 | 13 |
|CE-CS-SS | 2  |  5 | 4/10 |
| RST | 1 |  | 3 |

LCD Nokia 5110

## Nokia 5110 ##
Połączenia dla noki 5110
  * nr\_pin\_lcd - Nazwa - nr\_pin\_arduino
  * 1- rst - 3
  * 2 -ce - 4
  * 3- dc - 5
  * 4- din - 6
  * 5- clk - 7
  * 6- vcc
  * 7- light
  * 8- gnd
  * 3,3 V

## SD Card ##
  * Connect CLK to pin 13
  * Connect DO to pin 12
  * Connect DI to pin 11
  * Connect CS to pin 10
  * 3,3 V

# I2C #
  * BMP085 - 3,3 V
  * RTC module - 5 V

  * A4 - SDA
  * A5 - SCL


// Connect VCC of the BMP085 sensor to 3.3V (NOT 5.0V!)
// Connect GND to Ground
// Connect SCL to i2c clock - on '168/'328 Arduino Uno/Duemilanove/etc thats Analog 5
// Connect SDA to i2c data - on '168/'328 Arduino Uno/Duemilanove/etc thats Analog 4
// EOC is not used, it signifies an end of conversion
// XCLR is a reset pin, also not used here
/////////////SD card
//GND
//uint8\_t const MISO\_PIN = 12; MISO - 12
//uint8\_t const SCK\_PIN = 13; SCK - 13
//uint8\_t const MOSI\_PIN = 11; MOSI - 11
//uint8\_t const SS\_PIN = 10; -> CS - 10
// 5V
// 3V
// GND

// pin 7 - Serial clock out (SCLK)
// pin 6 - Serial data out (DIN)
// pin 5 - Data/Command select (D/C)
// pin 4 - LCD chip select (CS)
// pin 3 - LCD reset (RST)