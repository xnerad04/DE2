# Lab 1: ADAM NERADILEK

### Morse code

1. Listing of C code which repeats one "dot" and one "comma" (BTW, in Morse code it is letter `A`) on a LED. Always use syntax highlighting, meaningful comments, and follow C guidelines:

```c
int main(void)
{
    // Set pin where on-board LED is connected as output
    pinMode(LED_GREEN, OUTPUT);

    // Infinite loop
    while (1)
    {
        // Generate a lettre `A` Morse code

        // WRITE YOUR CODE HERE
        digitalWrite(LED_GREEN, led_value);
        
        
        // Turn the LED on
        led_value = HIGH;
        
        // Dot duration
        _delay_ms(SHORT_DELAY);
        
        
        // Turn the LED off
        led_value = LOW;
        
        // Pause duration
        _delay_ms(SHORT_DELAY);   
        
        
        // Turn the LED on
        led_value = HIGH;  
        
        // Line duration
        _delay_ms(LONG_DELAY);        
        
        
        // Turn the LED off
        led_value = LOW;        

        // Pause between symbols
        _delay_ms(LONG_DELAY); 
    }

    // Will never reach this
    return 0;
}
```

2. Scheme of Morse code application, i.e. connection of AVR device, LED, resistor, and supply voltage. The image can be drawn on a computer or by hand. Always name all components and their values!

   ![your figure](https://github.com/xnerad04/DE2/blob/main/Lab1_homework.PNG)
