# Ethernet "2" Library for ESP32-Arduino core

Forked from https://github.com/adafruit/Ethernet2 but with minor edits to ensure W5500 works on ESP32.

***Note: Tested ONLY on ESP32.***

## ESP32 SPI Pin Configuration

This library uses the HSPI interface on ESP32. Connect your W5500 module as follows:

| W5500 Signal | ESP32 GPIO | HSPI Function |
|--------------|------------|---------------|
| MISO         | GPIO 12    | HSPI_MISO     |
| MOSI         | GPIO 13    | HSPI_MOSI     |
| SCLK         | GPIO 14    | HSPI_SCLK     |
| CS (SS)      | GPIO 15    | HSPI_SS       |

These pins are defined in `src/utility/w5500.h` and are used by default when initializing the Ethernet connection.

License
-------

Copyright (c) 2009-2016 Arduino LLC. All right reserved.

This library is free software; you can redistribute it and/or
modify it under the terms of the GNU Lesser General Public
License as published by the Free Software Foundation; either
version 2.1 of the License, or (at your option) any later version.

This library is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the GNU
Lesser General Public License for more details.

You should have received a copy of the GNU Lesser General Public
License along with this library; if not, write to the Free Software
Foundation, Inc., 51 Franklin St, Fifth Floor, Boston, MA 02110-1301 USA


[W5100]:                   http://www.wiznet.co.kr/product-item/w5100/
[W5500]:                   http://www.wiznet.co.kr/product-item/w5500/
