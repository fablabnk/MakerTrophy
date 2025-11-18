The aim here is to use a microcontroller to light and control a short LED strip. This will be used to fire light into the bottom of your acrylic design and light up the engraved parts. 

# Requirements:

- An Arduino Nano is provided/recommended as the microcontroller (although in theory any microcontroller can be used)
- Arduino IDE and Neopixel library are recommended on the software side
    - We recommend specifically "File -> Examples -> Adafruit Neopixel -> strandtest" as a starting point
- The microcontroller should be powered from a simple 5V USB charger. Use no more than 5 LEDs to avoid burnout (see below)
- The microcontroller, wiring and LED strip should fit well within your 3D printed base
- Electrical connections should be solid, so soldering lengths of wire in place will be needed (particularly on the LED strip itself)
- Fading and other effects are strongly encouraged :)

# Tips

- When flashing the Nano, In the Arduino IDE under "Tools Menu -> Processor" ensure you select "ATMega328P (Old Bootloader)"
- Ensure you're using a USB cable with a data wire
- The LED strip has adhesive to allow it to be mounted inside your 3D print. Alignment is key!
- Beware of bending the LED strip close to the connections when soldered, the pads can easily snap off!

# Basics of the circuit

We will use a very simple circuit here, which uses the Nano's 5V pin to power the LED strip. Note that this is only recommended for up to 5 LEDs as the 5V pin can only provide a max of 500mA. For any more than this, your LED strip should be and share a ground with the Arduino.

There are just three connections that go from the Arduino to the LED strip, as follows:
- Arduino 5V pin goes to LED strip +5V pad
- Arduino Pin D6 goes to LED strip Din pad. Other D pins can be used and this can be changed in your Arduino code
- Arduino GND pin goes to LED strip GND pad. Suggest to use GND closest to Arduino 5V pin






