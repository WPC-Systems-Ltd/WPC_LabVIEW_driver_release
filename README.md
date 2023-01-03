# WPC_LabVIEW_driver_release

## Installation

- For WPC_device_driver
Unzip and install .vip with [VIPM](https://www.vipm.io/download/)

Download LabVIEW 2015 SP1 [Run-time engine](https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view).  

## Examples

Examples are included in the package and accessible from the LabVIEW Example Finder.

## Products

Ethernet based motion card
- EMotion

Ethernet based DAQ card
- Ethan-A
- Ethan-D
- Ethan-L
- Ethan-O

USB interface DAQ card
- USB-DAQ-F1-D (Digital)
- USB-DAQ-F1-DSNK (24V Digital)
- USB-DAQ-F1-AD (Digital + AI)
- USB-DAQ-F1-TD (Digital + Thermocouple)
- USB-DAQ-F1-RD (Digital + RTD)
- USB-DAQ-F1-CD (Digital + CAN)
- USB-DAQ-F1-AOD (Digital + AI + AO)

Wifi based DAQ card
- Wifi-DAQ-E3-A

# I/O Function Table

| Model           | AI  | AO | DI         | DO         | CAN | UART | SPI | I2C  | RTD | Thermocouple | Motion |
|:----------------|:---:|:--:|:----------:|:----------:|:---:|:----:|:---:|:----:|:---:|:------------:|:------:|
| EMotion         | -   | -  | -          | -          |-    |-     |-    |-     | -   |-             | 0      |
| Ethan-A         | 0   | -  | -          | -          |-    |-     |-    |-     | -   |-             |-       |
| Ethan-D         | -   | -  | 1          | 0          |-    |-     |-    |-     | -   |-             |-       |
| Ethan-L         | -   | -  | 1          | 0          |-    |-     |-    |-     | -   |-             |-       |
| Ethan-O         | -   | 0  | -          | -          |-    |-     |-    |-     | -   |-             |-       |
| USB-DAQ-F1-D    | -   | -  | 0, 1, 2, 3 | 0, 1, 2, 3 |-    |1, 2  |1, 2 | 1, 2 | -   |-             |-       |
| USB-DAQ-F1-DSNK | -   | -  | 0, 1       | 2, 3       |-    |-     |-    |-     | -   |-             |-       |
| USB-DAQ-F1-AD   | 0   | -  | 0, 1, 2, 3 | 0, 1, 2, 3 |-    |1, 2  |2    | 1, 2 | -   |-             |-       |
| USB-DAQ-F1-TD   | -   | -  | 0, 1, 2, 3 | 0, 1, 2, 3 |-    |1, 2  |2    | 1, 2 | -   |1             |-       |
| USB-DAQ-F1-RD   | -   | -  | 0, 1, 2, 3 | 0, 1, 2, 3 |-    |1, 2  |2    | 1, 2 | 1   |-             |-       |
| USB-DAQ-F1-CD   | -   | -  | 0, 1, 2, 3 | 0, 1, 2, 3 |1    |1, 2  |2    | 1, 2 | -   |-             |-       |
| USB-DAQ-F1-AOD  | 0   | 0  | 0, 1, 2, 3 | 0, 1, 2, 3 |-    |1, 2  |-    | 1, 2 | -   |-             |-       |
| Wifi-DAQ-E3-A   | 1   | -  | -          | -          |-    |-     |-    |-     | -   |-             |-       |

Take `USB-DAQ-F1-AOD` for example:
- Port 0 is available for `AI`
- Port 2 is available for `DI`
- Ports 0 & 1 are available for `DO`
- Port 2 is available for `UART`
 

## License

**WPC LabVIEW driver release** is licensed under an MIT-style license see
[LICENSE](https://github.com/WPC-Systems-Ltd/WPC_LabVIEW_driver_release/blob/main/LICENSE). Other incorporated projects may be licensed under different licenses.
All licenses allow for non-commercial and commercial use.

