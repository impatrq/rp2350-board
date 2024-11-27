# rp2350-board

## Hardware

### Conexiones tentativas

#### RP2040-Zero

| GPIO | Función | Conexión Principal | Conexión Secundaria | Descripción |
| --- | --- | --- | --- | --- |
| 0 | UART0 TX | RP2350 UART0 RX | - | Comunicación UART entre Picos |
| 1 | UART0 RX | RP2350 UART0 TX | - | Comunicación UART entre Picos |
| 2 | - | RP2350 SWCLK | - | Linea de clock para debugger |
| 3 | - | RP2350 SWD | - | Linea de datos para debugger |
| 4 | I2C1 SDA | RP2350 I2C1 SDA | - | Línea de datos de I2C entre Picos |
| 5 | I2C1 SCL | RP2350 I2C1 SCL | - | Línea de clock de I2C entre Picos |
| 6 | GP6 | J2 | - | GPIO |
| 7 | GP7 | J2 | - | GPIO |
| 8 | GP8 | J2 | - | GPIO |
| 9 | GP9 | J2 | - | GPIO |
| 10 | GP10 | J2 | - | GPIO |
| 11 | GP11 | J2 | - | GPIO |
| 12 | GP12 | J2 | - | GPIO |
| 13 | GP13 | J2 | - | GPIO |
| 14 | GP14 | J2 | - | GPIO |
| 15 | GP15 | J2 | - | GPIO |
| 26 | ADC0 | J2 | - | Canal 0 de ADC del RP2040 |
| 27 | ADC1 | J2 | - | Canal 1 de ADC del RP2040 |
| 28 | ADC2 | J2 | - | Canal 2 de ADC del RP2040 |
| 29 | ADC3 | J2 | - | Canal 3 de ADC del RP2040 |

#### RP2350

| GPIO | Función | Conexión Principal | Conexión Secundaria | Descripción |
| --- | --- | --- | --- | --- |
| 0 | UART0 TX | RP2040 UART0 RX | - | Comunicación UART externa |
| 1 | UART0 RX | RP2040 UART0 TX | - | Comunicación UART externa |
| 2 | INPUT | SW0 | - | Pulsador con pull-up |
| 3 | INPUT | SW1 | - | Pulsador con pull-up |
| 4 | I2C0 SDA | SDA | J4 | Comunicación por I2C con dispositivos internos |
| 5 | I2C0 SCL | SCL | J4 | Comunicación por I2C con dispositivos internos |
| 6 | GP6 | | | |
| 7 | GP7 | | | |
| 8 | GP8 | UART1 TX | - | Comunicación por UART para ESP-01 |
| 9 | GP9 | UART1 RX | - | Comunicación por UART para ESP-01 |
| 10 | GP10 | LED1 | - | Salida para LED Verde |
| 11 | GP11 | LED2 | - | Salida para LED Amarillo |
| 12 | GP12 | LED3 | - | Salida para LED Rojo |
| 13 | GP13 | LED RGB RED | - | Salida LED RGB Rojo |
| 14 | GP14 | LED RGB GREEN | - | Salida LED RGB Verde |
| 15 | GP15 | LED RGB BLUE | - | Salida LED RGB Azul |
| 16 | SPI0 MISO | MISO | - | Comunicación por SPI con dispositivos internos |
| 17 | SPI0 CS0 | CS0 | - | Comunicación por SPI con dispositivos internos |
| 18 | SPI0 SCK | SCK | - | Comunicación por SPI con dispositivos internos |
| 19 | SPI0 MOSI | MOSI | - | Comunicación por SPI con dispositivos internos |
| 20 | GP20 | J3 | | GPIO |
| 21 | GP21 | J3 | | GPIO |
| 22 | GP22 | J3 | | GPIO |
| 23 | GP23 | J3 | | GPIO |
| 24 | GP24 | J3 | | GPIO |
| 25 | GP25 | J3 | | GPIO |
| 26 | GP26 | J3 | | GPIO |
| 27 | GP27 | J3 | | GPIO |
| 28 | GP28 | J3 | | GPIO |
| 29 | GP29 | J3 | | GPIO |
| 30 | GP30 | J3 | | GPIO |
| 31 | GP31 | J3 | | GPIO |
| 32 | GP32 | J3 | | GPIO |
| 33 | GP33 | J3 | | GPIO |
| 34 | GP34 | J3 | | GPIO |
| 35 | GP35 | J3 | | GPIO |
| 36 | GP36 | J3 | | GPIO |
| 37 | GP37 | J3 | | GPIO |
| 38 | GP38 | J3 | | GPIO |
| 39 | GP39 | J3 | | GPIO |
| 40 | ADC0 | J4 | RV1 | Canal 0 de ADC del RP2350 |
| 41 | ADC1 | J4 | RV2 | Canal 1 de ADC del RP2350 |
| 42 | ADC2 | J4 | | Canal 2 de ADC del RP2350 |
| 43 | ADC3 | J4 | | Canal 3 de ADC del RP2350 |
| 44 | ADC4 | J4 | | Canal 4 de ADC del RP2350 |
| 45 | ADC5 | J4 | | Canal 5 de ADC del RP2350 |
| 46 | ADC6 | J4 | | Canal 6 de ADC del RP2350 |
| 47 | ADC7 | J4 | | Canal 7 de ADC del RP2350 |

#### Dispositivos de I2C

| Módulo | Bus de I2C | Descripción |
| --- | --- | --- |
| BH1750 | RP2350 I2C0 | Sensor de luz |
| SSD1306 | RP2350 I2C0 | OLED 128x32 |
| BMP180 | RP2350 I2C0 | Sensor de presión y temperatura |

#### Dispositivos de SPI

| Módulo | Bus de SPI | Descripción |
| --- | --- | --- |
| SD | SPI0 | Módulo de tarjeta SD |
| MAX6675 | SPI0 | Interfaz para termocupla tipo K |
