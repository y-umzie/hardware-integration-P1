# hardware-integration-P1
This repo contains the code as well as other details of the project

Step 1: Circuit Diagram
Here’s how you should connect your components:
1.	Adafruit Feather nRF52840 Express:
o	Green LED: Connect the anode to a GPIO pin (e.g., D5) and the cathode to GND.
o	Red LED: Connect the anode to another GPIO pin (e.g., D6) and the cathode to GND.
o	BME280 Sensor: Connect VCC to 3.3V, GND to GND, SCL to SCL, and SDA to SDA.

Step 2: Code
Below is the Arduino code to achieve the functionality you described:
{
    Find the code in the other files
}

Step 3: Flashing the Code
To flash the code using JTAG:
1.	Install J-Link Software: Download and install the J-Link software from SEGGER’s website.
2.	Connect JTAG: Connect the JTAG to your Adafruit Feather nRF52840 Express.
3.	Arduino IDE Setup:
o	Go to Tools > Board > Boards Manager and install the Adafruit nRF52 board package.
o	Select Adafruit Feather nRF52840 Express from the board list.
o	Go to Tools > Programmer and select J-Link.
4.	Upload Code: Click on the upload button in the Arduino IDE to flash the code to your board.

Documentation
1.	Power ON: When the power switch is turned on, the green LED will light up for 1 second if the battery is connected.
2.	Sensor Check: If the BME280 sensor is not connected, the red LED will light up for 1 second and the device will advertise an error via Bluetooth.
3.	Data Collection: If the sensor is connected, it will collect pressure, temperature, and humidity data and publish it over Bluetooth.

<h1>**Components**</h1>
<ul>Adafruit Feather nRF52840 Express
GY-BME20-5V Sensor
Green LED
Red LED
Resistors (220Ω for LEDs)
Breadboard and Jumper Wires</ul>

<h2>nRF52840</h2>
<ul>
    It is a SoC(System on Chip) developed by Nordic Semiconductors.
It is available in various forms depending on the use such as Stand alone SoC, Dongle and Development Kit (DK).
It is built around ARM Cortex-M4 CPU with 1MB of flash memory and 256KB of RAM.
nRF – n stand for Nordic; RF for Radio Frequency 
The Development Kit is a versatile single-board development kit which comes with an NFC antenna.
</ul>

<h2>Adafruit Feather nRF52840</h2>
![image](https://github.com/user-attachments/assets/652c3fc7-fea4-439d-ac0f-1a5777ffda35)
<ul>A development board from Adafruit that have 1MB flash and 256KB SRAM
It is compatible with both Arduino and BLE with built-in USB plus battery charging
It comprises 21 GPIO, 6 x 12-bit ADC pins, upto 12 PWM outputs
</ul>
