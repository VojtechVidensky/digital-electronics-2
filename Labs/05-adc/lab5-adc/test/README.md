# Lab 5: Vojtěch Vídenský

### Analog-to-Digital Conversion

1. Complete table with voltage divider, calculated, and measured ADC values for all five push buttons.

   | **Push button** | **PC0[A0] voltage** | **ADC value (calculated)** | **ADC value (measured)** | **ADC value (measured, hex)** |
   | :-: | :-: | :-: | :-: | :-: |
   | Right  | 0&nbsp;V | 0   | 0 | 0 |
   | Up     | 0.495&nbsp;V | 101 | 99 | 63 |
   | Down   | 1.203&nbsp;V | 246 | 257 | 101 |
   | Left   | 1.969&nbsp;V | 402 | 409 | 199 |
   | Select | 3.181&nbsp;V | 651 | 639 | 27f |
   | none   | 5&nbsp;V | 1023 | 1023 | 3ff |

### Temperature meter

Consider an application for temperature measurement. Use analog temperature sensor [TC1046](http://ww1.microchip.com/downloads/en/DeviceDoc/21496C.pdf), LCD, and a LED. Every 30 seconds, the temperature is measured and the value is displayed on LCD screen. When the temperature is too high, the LED will turn on.

2. Draw a schematic of temperature meter. The image can be drawn on a computer or by hand. Always name all components and their values.

   ![image](https://user-images.githubusercontent.com/99399676/199074447-67c3e93c-e23c-40af-b230-b719f834d2fd.png)

3. Draw two flowcharts for interrupt handler `TIMER1_OVF_vect` (which overflows every 1&nbsp;sec) and `ADC_vect`. The image can be drawn on a computer or by hand. Use clear descriptions of the individual steps of the algorithms.

   ![image](https://user-images.githubusercontent.com/99399676/199075862-41ae3bec-c68f-4a62-a1c8-666b6b53fc6d.png)

