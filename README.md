# Introduction

​The high-speed USB adapter chip CH347 is a conversion chip integrating 480Mbps high-speed USB interface, JTAG interface, SPI interface, I2C interface, asynchronous UART serial port, GPIO interface and other hardware interfaces.

Interface diagram:

![img](README.assets/6c32c76c1cff4c5aaeb09e9334cad8c7.png)

Application diagram:

![img](README.assets/e36f121404b04ae28f82a863b6036342.png)

## JTAG interface features

- Work in Host/Master host mode
- Hardware signals: TMS, TCK, TDI, TDO and TRST
- Support fast mode and bit-bang mode of custom protocol, the transmission rate can reach 30Mbit/S
- Provide computer-side driver and USB to JTAG TAP function library to support secondary development

## SPI interface features

Work in Host/Master host mode
- Built-in hardware DMA, supports fast sending and reading of bulk data
- Hardware signals: SCS0, SCS1, SCK, MISO and MOSI
- Working mode: SPI mode 0/SPI mode 1/SPI mode 2/SPI mode 3
- Transmission bit sequence: MSB/LSB
- Data structure: 8-bit/16-bit transmission
- Provide computer-side driver and USB-to-SPI function library to support secondary development

## I2C Interface Features

- Work in Host/Master host mode
- Hardware signal: SCL, SDA
- Support 4 transmission speeds: low speed 20KHz, standard 100KHz, fast 400KHz, high speed 750KHz
- Support I2C timing parameter adjustment
- Provide computer-side driver and USB to I2C function library to support secondary development

## UART interface features

Hardware signal: TXD, RXD, Modem signal
- Support serial port baud rate: 1200bps~9Mbps
- Support serial port data format: 8 data bits, 1/2 stop bits, odd/even/no parity
- Support RS485 direction automatic switching
- Support serial port automatic hardware flow control
- Provide VCP serial port driver mode/HID driver-free application mode
- Support standard serial port/manufacturer CH347 dynamic library/HID interface to access serial port

# project instruction

This project will gradually add features. Currently working:

1. Add the Openocd executable environment of CH347-JTAG interface

2. Relying on the FPGA download tool CH347FPGADownloader written by openocd in 1, it is currently possible to program some FPGAs of XILINX.
