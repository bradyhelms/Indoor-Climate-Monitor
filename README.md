## Indoor Climate Monitor

This project is an **indoor climate monitor** built on the **NUCLEO-F446RE** development board. It's designed to continuously measure and display environmental data. The system integrates a digital temperature and humidity sensor with an LCD screen to provide real-time readings. 

***

### Key Components

* **NUCLEO-F446RE**: The central processing unit for the system. This board provides the necessary computational power and peripherals to interface with the sensors and display.
* **DHT22 Sensor**: A reliable sensor for measuring **temperature** and **humidity**. It uses a single-wire protocol, implemented via a UART interface, for communication with the microcontroller.
* **I2C LCD**: A liquid crystal display that uses the **I2C communication protocol**. This screen serves as the primary output, showing the measured climate data in a user-friendly format.

***

### Functionality

The main function of the device is to read data from the DHT22 sensor and display it on the LCD. The system is programmed to:

1.  Initialize the necessary peripherals on the STM32 microcontroller, including the UART for the DHT22 and the I2C for the LCD.
2.  Continuously query the DHT22 sensor for the current temperature and humidity readings.
3.  Process the sensor data and format it for display.
4.  Update the I2C LCD with the most recent temperature and humidity values.
