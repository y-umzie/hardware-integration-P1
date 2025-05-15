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
