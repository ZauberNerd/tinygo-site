---
title: 'ST Micro "Nucleo" L031K6'
weight: 3
---

The [STM32 Nucleo L031K6](https://www.st.com/en/evaluation-tools/nucleo-l031k6.html) is an ARM development board based on the ST Micro [STM32L031K6](https://www.st.com/en/microcontrollers-microprocessors/stm32l031k6.html) SoC.

It has 2 user buttons, and 3 user LEDs.

## Interfaces

| Interface | Hardware Supported | TinyGo Support |
| --------- | ------------- | ----- |
| GPIO      | YES | YES |
| UART      | YES | YES |
| SPI      | YES | YES |
| I2C      | YES | YES |
| ADC      | YES | Not yet |
| PWM      | YES | Not yet |

## Machine Package Docs

[Documentation for the machine package for the STM32 Nucleo L031K6](../machine/nucleo-l031k6)

## Flashing

### OpenOCD

Programs are loaded onto the STM32 Nucleo L031K6 with the onboard [STLink v2](https://www.st.com/en/development-tools/st-link-v2.html) hardware programmer, using the `openocd` command line utility program to perform the board flashing. You must install [OpenOCD](http://openocd.org/) before you will be able to flash the STM32 Nucleo L031K6 board with your TinyGo code.

- Plug your STM32 Nucleo L031K6 into your computer's USB port.
- Build and flash your TinyGo program using `tinygo flash -target=nucleo-l031k6`
