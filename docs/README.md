## Welcome to Micro Controller Peripherals in Ada

This site lists various micro-controller boards that can be used with the programming language Ada. Currently we are focused on AVR boards as we have an Ada compiler only for these processors.  We are planning to extend it to also cover ESP8266 and ESP32 boards.

### Boards

- Arduino Uno (atmega328p)
- Arduino Nano V3 (atmega328p)
- _ESP-01_ (esp8266)

### AVR Internal Units

- 8bit Timers
- 16bit Timers
- UART for Serial Communication
- Analog/Digital Converter (ADC)

### Input Devices

- Key
- Potentiometer (variable resistor)
- Voltage Meter
- One-Wire
  - Temperature Sensor 18B20
- DHT22, Temperature / Humidity Sensor


### Output Devices

- LED
- IO Expander
- Displays
  - Single 7-Segment Digit
  - 4 7-Segment Digits
  - 2 lines of 4 7-segment digits
  - LCD 1602 (2 lines of 16 characters), directly driven
  - LCD 2004 (4 lines of 20 characters), via IO expander

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

#### Sytax highlighting of Ada code
```ada
with Ada.Text_IO;    use Ada.Text_IO;
procedure Hello is
begin
   Put_Line ("Hello World!");
end Hello;
```
   
### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/RREE/mc_peripherals_in_ada/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
