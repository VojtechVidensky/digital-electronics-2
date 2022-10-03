# Lab 1: Vojtěch Vídenský

### Morse code

1. Listing of C code which repeats one "dot" and one "comma" (BTW, in Morse code it is letter `A`) on a LED. Always use syntax highlighting, meaningful comments, and follow C guidelines:

```c

#define LED_RED PB0
#define SHORT_DELAY 250 // Delay in milliseconds
#define LONG_DELAY 500
#define PB0 8

int main(void)
{
    uint8_t led_value = LOW;  // Local variable to keep LED status

    // Set pin where on-board LED is connected as output
    pinMode(LED_RED, OUTPUT);

    // Infinite loop
    while (1)
    {
        digitalWrite(LED_RED, HIGH);
        _delay_ms(SHORT_DELAY);
        digitalWrite(LED_RED, LOW);
        _delay_ms(SHORT_DELAY);
        digitalWrite(LED_RED, HIGH);
        _delay_ms(SHORT_DELAY);
        digitalWrite(LED_RED, LOW);
        _delay_ms(LONG_DELAY);
        digitalWrite(LED_RED, HIGH);
        
    }

    // Will never reach this
    return 0;
}
```

2. Scheme of Morse code application, i.e. connection of AVR device, LED, resistor, and supply voltage. The image can be drawn on a computer or by hand. Always name all components and their values!

   ![image](https://user-images.githubusercontent.com/99399676/193632515-9c7d7a4c-a3b3-4656-88b6-f9bde81d51d5.png)
