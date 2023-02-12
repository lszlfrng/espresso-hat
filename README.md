# Espresso-HAT-EEP

Basic espresso machine control board with [WeAct Studio STM32F411CEU6 BlackPill](https://stm32-base.org/boards/STM32F411CEU6-WeAct-Black-Pill-V2.0.html) extension board. Is good for Gaggiuino project also.

## Originality 

The project based on GaggiaBoard_V3 which is part of the [CoffeeHat](https://github.com/banoz/CoffeeHat) repository created by [banoz](https://github.com/banoz). 
Please visit [banoz's CoffeeHat](https://github.com/banoz/CoffeeHat) project for information and improvements. 

## Changes

Compared to [Original](https://github.com/banoz/CoffeeHat/tree/5b03bb7c6b7397ed60ee60732e1ad4fe17a17d7e)
* ported from Eagle to JLCEDA Pro (EasyEDA Pro)
* few track changes
* fixed (or modified) some part's LCSC part number.

## Connectors

Copied from original documentation

Supports 3-Way valve control, PSM control for a vibe pump based on zero-crossing detector, Qwiic I2C connector for various peripherals (e.g. displays, thermal sensors), header breakout for Black Pill pins.

```
J10, J11 - AC input
J12 - pump
J13 - 3-way valve

J1 - UART2 (PA2/PA3)
J2 - I2C
J4 - thermocouple
J6 - Pressure sensor (ADS101X/ADS111X on I2C1)
J7 - Brew (PC14) / Steam (PC15) switch
J8 - Scales (PB0 -> CLK, PB8 -> D1, PB9 -> D2)
J9 - 5V SSR control (PA15 -> SSR1, PA8 -> SSR2)

AC zero-cross sense on PA0
Pump control on PA1
3-Way valve control on PC13

SPI1 is used by thermocouple amplifier on PA5(SPI1_SCK)/PB4(SPI1_MISO), and CS on PA6

I2C port on PB6(I2C1_SCL)/PB7(I2C1_SDA)

J27 - USART1 (PA9/10) with NRST and BOOT1
```

DISCLAIMER

This project is provided AS-IS, use at your sole discretion and your own risk. Parts of this project can work under dangerous voltages and require special care. Please don't do anything you're not sure about. The maintainer(s) can not be held liable for any suffer or loss or harm or anything else.
