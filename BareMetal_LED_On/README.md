
# STM32F411RE Bare-Metal LED Blinking

This project demonstrates LED blinking on the STM32F411RE microcontroller using bare-metal programming without HAL libraries.

## Overview

The program directly accesses STM32 peripheral registers to:

- Enable GPIOA peripheral clock
- Configure PA5 as Output Mode
- Toggle the onboard LED connected to PA5
- Generate delay using a software loop

## Hardware

- STM32 Nucleo-F411RE
- STM32F411RE Microcontroller
- Onboard User LED (PA5)

## Software

- STM32CubeIDE
- Embedded C
- Bare-Metal Programming

## GPIO Configuration

| Pin | Mode | Function |
|------|------|----------|
| PA5 | Output | User LED |

## Working Principle

1. Enable GPIOA clock using RCC register.
2. Configure PA5 as General Purpose Output.
3. Set PA5 HIGH.
4. Delay.
5. Set PA5 LOW.
6. Delay.
7. Repeat indefinitely.

## Register-Level Operations

- RCC_AHB1ENR
- GPIOA_MODER
- GPIOA_ODR

## Learning Objectives

- Understanding STM32 memory-mapped registers
- GPIO configuration without HAL
- Bitwise operations in Embedded C
- Bare-metal embedded programming concepts

## Target Board

STM32 Nucleo-F411RE

## Author

SID
