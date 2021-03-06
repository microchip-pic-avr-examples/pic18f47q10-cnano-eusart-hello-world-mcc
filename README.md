[![MCHP](images/microchip.png)](https://www.microchip.com)

# EUSART Sending "Hello World" message

This example shows how to send a string message from the PIC18F47Q10 microcontroller to the PC and use MPLAB Data Visualizer Terminal to see it.

## Related Documentation

- [TB3282 - Getting Started with UART using EUSART on PIC18](https://www.microchip.com/wwwappnotes/appnotes.aspx?appnote=en1003086)
- [PIC18F-Q10 Family Product Page](https://www.microchip.com/design-centers/8-bit/pic-mcus/device-selection/pic18f-q10-product-family)
- [PIC18F47Q10 Data Sheet](http://ww1.microchip.com/downloads/en/DeviceDoc/40002043D.pdf)
- [PIC18F47Q10 Code Examples on GitHub](https://github.com/microchip-pic-avr-examples?q=pic18f47q10-cnano&type=&language=)

## Software Used

- MPLAB® X IDE 5.45 or newer [(microchip.com/mplab/mplab-x-ide)](http://www.microchip.com/mplab/mplab-x-ide)
- MPLAB® XC8 2.31 or newer [(microchip.com/mplab/compilers)](http://www.microchip.com/mplab/compilers)
- MPLAB® Code Configurator (MCC) 4.1.0 or newer [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
- MPLAB® Melody Library 1.37.18 or newer [(microchip.com/mplab/mplab-code-configurator)](https://www.microchip.com/mplab/mplab-code-configurator)
- Microchip PIC18F-Q Series Device Support 1.8.154 or newer [(packs.download.microchip.com/)](https://packs.download.microchip.com/)

## Hardware Used

- PIC18F47Q10 Curiosity Nano [(DM182029)](https://www.microchip.com/Developmenttools/ProductDetails/DM182029)

## Setup

The PIC18F47Q10 Curiosity Nano Development Board [(DM182029)](https://www.microchip.com/Developmenttools/ProductDetails/DM182029) is used as the test platform. It has an onboard debugger that acts as an USART to USB convertor so no further hardware is needed.

The following configurations must be made for this project:

CLKCTRL: default

EUSART2:
- Transmit Enabled
- Serial Port Enabled
- Baud Rate: 9600

Clock Control:
- Clock Source: HFINTOSC
- HF Internal Clock: 4_MHz
- Clock Divider: 4

Configuration Bits:
- WDT Operating Mode: WDT Disabled


## Operation

Run the code, start MPLAB® X Data Visualizer on the correct COM port and select the terminal input source than messages will start appearing.

![Demo in MPLABX Data Visualizer](./images/demo.png)>

## Summary

In this example the EUSART is set in the most common configuration (asynchronous operation and 8N1 message format) and "Hello World" messages are transmitted. Data Visualizer is used to see the messages on the PC.
