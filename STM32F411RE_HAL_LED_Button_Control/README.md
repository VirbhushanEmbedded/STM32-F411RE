# STM32F411RE HAL LED Button Control

This project demonstrates controlling an LED using a push button on the STM32F411RE microcontroller with the STM32 HAL (Hardware Abstraction Layer) library.

## Overview

The program reads the state of the user push button and controls the onboard LED accordingly. When the button is pressed, the LED changes state based on the implemented logic.

## Hardware

- STM32 Nucleo-F411RE
- STM32F411RE Microcontroller
- Onboard User LED (PA5)
- User Push Button (PC13)

## Software

- STM32CubeIDE
- STM32 HAL Library
- Embedded C

## GPIO Configuration

| Pin | Mode | Function |
|------|------|----------|
| PA5 | Output Push-Pull | User LED |
| PC13 | Input | User Button |

## Working Principle

1. Initialize the HAL Library.
2. Configure the system clock.
3. Initialize PA5 as GPIO Output.
4. Initialize PC13 as GPIO Input.
5. Read button state using HAL_GPIO_ReadPin().
6. Control the LED using HAL_GPIO_WritePin().
7. Repeat indefinitely.

## Key HAL Functions Used

- HAL_Init()
- SystemClock_Config()
- MX_GPIO_Init()
- HAL_GPIO_ReadPin()
- HAL_GPIO_WritePin()

## Learning Objectives

- GPIO input configuration
- GPIO output control
- Reading push button status
- Using HAL APIs for digital I/O
- Basic embedded systems development

## Target Board

STM32 Nucleo-F411RE

## Author

virbhushan
