# LED

The simplest output device on a micro controller. A LED can typically be connected directly to a GPIO pin. Use an appropriate resistor to limit the current (100 .. 1k).

![LED](../img/LED_100.jpg)


## Ada

GPIOs are handled as boolean variables. Off (dark) and on (light) depend on your wiring. If the LED is between a GPIO and ground the GPIO must have high level to switch the LED on.  If the LED is between a GPIO and Vcc the GPIO must have low level to switch the LED on. I recommend to redefine On and Off as renamings of True and False.

```ada
   -- define On and Off for a LED between GPIO and Ground.
   function On return Boolean renames True;
   function Off return Boolean renames False;
   
   -- set the pin for the LED
   -- there is a LED on the Arduino platform at Port B, pin 5 (digital pin 13)
   LED    : Boolean renames AVR.MCU.PORTB_Bits (5);
   LED_DD : Boolean renames AVR.MCU.DDRB_Bits (5);
   
   -- set the GPIO as output
   LED_DD := DD_Output; 
   
   -- switch the LED on
   LED := On;
```

See the files [`LED.ads`](https://sourceforge.net/p/avr-ada/code/ci/master/tree/apps/delays/led.ads) and [`LED.adb`](https://sourceforge.net/p/avr-ada/code/ci/master/tree/apps/delays/led.adb) in AVR-Ada for a bit more elaborate example, still producing only single assembler commands.