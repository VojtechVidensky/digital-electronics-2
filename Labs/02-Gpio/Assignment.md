# Lab 2: Vojtěch Vídenský

### GPIO control registers

1. Complete the table for DDRB and PORTB control register values.

   | **DDRB** | **PORTB** | **Direction** | **Internal pull-up resistor** | **Description** |
   | :-: | :-: | :-: | :-: | :-- |
   | 0 | 0 | input | no | Tri-state, high-impedance |
   | 0 | 1 | input | yes | Activation of pull-up rezistor |
   | 1 | 0 | Output | no | Output low (sink) |
   | 1 | 1 | Output | no | Output high (source) |

### GPIO library

2. Complete the table with code sizes from three versions of the blink application.

   | **Version** | **Size [B]** |
   | :-- | :-: |
   | Arduino-style     | 480 |
   | Registers         | 182 |
   | Library functions | 178 |

### Traffic light

3. Scheme of traffic light application with one red/yellow/green light for cars, one red/green light for pedestrians, and one push button. Connect AVR device, LEDs, resistors, push button (for pedestrians), and supply voltage. The image can be drawn on a computer or by hand. Always name all components and their values!

   ![image](https://user-images.githubusercontent.com/99399676/194276732-5fc1eaf5-eed5-4227-9c52-2574ace821f8.png)


