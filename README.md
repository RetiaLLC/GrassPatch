# Grass Patch board resources

This repo contains a schematic for the module, as well as datasheets for all of the important components!

What are you getting?

* A USB Nugget, with its:
 * WiFi and Bluetooth capabilities
 * 128x64 SH1106 OLED display
 * 4 clicky buttons
 * A Neopixel LED

It's mounted onto a patch of grass, on which you'll find:

* a (pretty loud) buzzer with MIDI playback support
* an LED bargraph driven from an I2C IO expander
* a LoRa modem from SeeedStudio, based on the SX1262 chip with wide software support
* an infrared transmitter-receiver pair that can make two boards talk together
* a temperature sensor hidden inside of a ball of yarn
* an extra sensor port for I2C sensors of your choice!

# How to get at it?

- Install [Thonny](https://thonny.org/) on your computer

- If we haven't done this already - [download and flash MicroPython](https://micropython.org/download/LOLIN_S2_MINI/) onto your Nugget

- Upload `hw.py` and `sh1106.py` - they're hardware support libraries

- Upload `main.py` and see it play a melody

- Hack away at `main.py` to play with the onboard devices and sensors!

  Notes:
-  Some components, like the compass and the LoRa modem, will require libraries. For the compass, you can [try out this library](https://github.com/gvalkov/micropython-esp8266-hmc5883l/blob/main/hmc5883l.py), and for the LoRa modem, feel free to refer to one of the SX1262 libraries!
-  Peruse the files in the `datasheets/` folder to learn more about the components
