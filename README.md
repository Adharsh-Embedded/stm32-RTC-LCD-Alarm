# STM32 RTC Alarm Clock with LCD

A simple RTC-based Alarm Clock using the STM32 Nucleo-F446RE. The project displays the current time and date on a 16x2 I2C LCD, allows the user to set an alarm using push buttons, and turns on an LED when the alarm time is reached.

## Features

- Real-Time Clock (RTC) using STM32 RTC peripheral
- Displays current time and date on 16x2 I2C LCD
- Set alarm hour using a push button
- Set alarm minute using a push button
- Enable alarm using a push button
- LED and Buzzer indication when alarm time matches RTC time
- UART debugging support

## Hardware Required

- STM32 Nucleo-F446RE
- 16x2 LCD with I2C module
- 3 Push Buttons
- LED (or onboard LED)
- Jumper wires

## Pin Connections

| Device | STM32 Pin |
|----------|----------|
| LCD SDA | PB9 |
| LCD SCL | PB8 |
| Hour Set Button | PC13 |
| Minute Set Button | PA0 |
| Alarm Enable Button | PB0 |
| Alarm LED | PA5 |
| UART2 TX | PA2 |
| UART2 RX | PA3 |

## How It Works

1. The LCD displays the current RTC time and date.
2. Press the Hour Set button (PC13) to increment the alarm hour.
3. Press the Minute Set button (PA0) to increment the alarm minute.
4. Press the Alarm Enable button (PB0) to start alarm monitoring.
5. When the RTC time matches the alarm time, the LED connected to PA5 turns ON.

## Peripherals Used

- GPIO
- RTC
- I2C1
- USART2

## Project Output

- Displays live time and date on LCD
- Displays configured alarm time
- Turns ON LED and Buzzer when alarm time is reached

## Future Improvements

- Store alarm settings in backup registers
- Support multiple alarms
- Add AM/PM mode

## Author

Adharsh
