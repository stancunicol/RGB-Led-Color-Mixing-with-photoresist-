![image](https://github.com/user-attachments/assets/8d4126bb-d03f-41d7-b22e-2f263b64ad6b)

# 🌈 Arduino RGB LED Color Mixer with Light Sensor Control
This Arduino project allows you to mix colors using three potentiometers and control the timing/delay of color transitions using a light sensor (LDR). The RGB LED’s color intensity is set by the potentiometers, while the ambient light (read from the light sensor) controls the pause duration between color changes.

# 🧰 Components Used
1 x Arduino UNO

1 x Breadboard

3 x 10kΩ Potentiometers

1 x RGB LED (common cathode)

3 x 220Ω Resistors (for each RGB pin)

1 x Light Sensor (LDR)

1 x 10kΩ Resistor (for the LDR voltage divider)

Jumper wires

USB cable for uploading code

# 🔌 Circuit Overview
RGB LED Pins:

Red → Pin 11 through 220Ω resistor

Green → Pin 10 through 220Ω resistor

Blue → Pin 9 through 220Ω resistor

Cathode → GND

Potentiometers:

Connected to analog pins A0, A1, A2

Used to control red, green, and blue values respectively

LDR (Light-Dependent Resistor):

Forms a voltage divider with a 10kΩ resistor

Connected to analog pin A3

Controls the delayTime between transitions (based on light intensity)

# 💡 Functionality
The three potentiometers control the RGB color intensity.

The light sensor reads ambient light and maps it to a delay time (50–2000 ms).

The LED will display the custom color, then briefly change to a fixed color (RGB = 255, 255, 102) before returning to user-controlled values after the light-based delay.
