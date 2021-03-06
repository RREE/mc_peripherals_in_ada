## Welcome to Micro Controller Peripherals in Ada

This site lists various micro-controller boards that can be used with the programming language Ada. Currently we are focused on AVR boards as we have an Ada compiler only for these processors.  We are planning to extend it to also cover ESP8266 and ESP32 boards.

### Boards

- AVR [Butterfly](/boards/butterfly) (atmega169)
- Arduino [Uno](/boards/arduino_uno) (atmega328p)
- Arduino [Nano](/boards/arduino_nano) V3 (atmega328p)
- [Digispark](/boards/digispark) (attiny85)
- [_ESP-01_](/boards/esp01) (esp8266)
- [_Wemos / Lolin D1 Mini_](/boards/wemos_d1_mini) (esp8266)
- [_ESP32_](/boards/esp32) (esp-32)

### AVR Internal Units

- GPIO
- Interrupts triggered at GPIOs
- 8bit Timers
- 16bit Timers
- UART for Serial Communication
- Analog/Digital Converter (ADC)
- I2C Bus Master

### Input Devices

- Keys
  - Single [Button](/input/button)
  - [Potentiometer](/input/poti) (variable resistor)
  - [Dual Axis Joystick](/input/dual_axis)
  - [Playstation PS2 Controller](/input/ps2)
  - [Capacitive Touch Sensor](/input/touch)
- Voltage Meter
- Current Sensor [INA219](/input/ina219)
- Temperature Sensors 
  - One-Wire Sensor [18B20](/input/18b20)
- Temperature and Humidity Sensors
  - [DHT22](/input/dht22)
- Temperature and Pressure Sensors
  - [BMP180](/input/bmp180)
  - [BMP280](/input/bmp280)


### Output Devices

- [LED](/output/LED.md)
- IO Expander [PCF8574](/output/pcf8574), I2C
- Displays
  - Single Digit 7-Segment 
  - 4 Digits 7-Segment 
  - 2 rows of 4 7-segment digits
  - LCD 1602 (2 lines of 16 characters), directly driven
  - LCD 2004 (4 lines of 20 characters), via I2C IO expander



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
