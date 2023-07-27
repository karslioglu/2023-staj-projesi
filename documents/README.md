# Tools to be used in the project
Communication protocols to be used in the project:
* UART:
UART (Universal Asynchronous Receiver Transmitter) is a comprehensive circuit that contains the necessary software to control the serial port of the computer. It can realize double-sided transmission by converting incoming parallel data to serial data or incoming serial data to parallel data. It works asynchronously and has a programmable structure. Data type and rate can be changed in this protocol.
* I2C:
I2C stands for Inter-Integrated Circuit. I2C is an example of synchronous communication from serial communication types. That is, data transmission is bidirectional, but data cannot be sent and received at the same time. Let's take radios as an example. It is preferred where minimum information exchange will take place. The bandwidth for communication is quite low. Apart from the ground line, two lines, SDA and SCL, are needed for communication. Due to the large number of lines, it is not preferred for long distance communications. It is generally used in places where short distance and low data transfer rate are sufficient. Supports master-slave communication. In I2C communication, there must be a master device controlling the communication and at least one slave device. The master decides which of the slave device connected to the line will transfer data.
* SPI
One of the most used serial communications is SPI, namely Serial Peripheral Interface communication.
SPI communication protocol works based on master/slave structure and allows full-duplex operation. 4 pins are required to perform SPI communication. These;

 MOSI (SDO) (Master Out Slave In)

 MISO (SDI) (Master In Slave Out)
 
 CS (SS) (Chip Select)
 
 Clock (SCL, CLK)
 
MOSI and MISO are the pins where we transfer data. With the CS pin, we are allowed to choose any slave device on the line. The clock pin, on the other hand, provides the transmission of data as a requirement for serial communication.

NOTE: Data transmission takes place in 8-bit.![](../../../spipng.png)
* GSM / GPS
Messaging systems and location features of mobile phones, which are indispensable in our daily life, can be given as examples. GSM communication protocol is the most important communication method for remote control systems. No matter where in the world, communication can be established between the two systems using SMS or voicemail. Again, the GPS system is the system used to find the instant location around the world. These two systems are already in every smartphone.

***The processor to be used in the project and the modules it will manage:***

* MCU: STM32F103R8T6:
"STM32F103C8T6" is a microcontroller model. It belongs to a popular 32-bit ARM Cortex-M3 microcontroller series manufactured by STMicroelectronics.

Below are the features and basic information of the STM32F103C8T6 microcontroller:

- Core: ARM Cortex-M3 core
- Operating Frequency: 72 MHz (some versions may have 36 MHz or other speeds)
- Memory: 64 KB Flash memory, 20 KB RAM
- Number of I/O Pins: 37 general purpose I/O pins
- Interrupt (IRQ) Processing: 16 interrupt lines (IRQ)
- Timers: 3 x 16-bit timers
- USART (UART): 3 x USART ports
- I2C: 2 I2C interfaces
- SPI: 2 SPI ports
- ADC: 12-bit, 16-channel ADC (Analog-to-Digital Converter)
- DMA: Direct Memory Access (DMA) controller
- Power Supply: operating voltage from 2.0V to 3.6V
- Package Type: LQFP-48

The STM32F103C8T6 is known as a popular microcontroller chip used in a wide range of applications such as industrial, medical, automotive and consumer electronics. It is preferred in many projects due to its advantages such as easy programmability, high performance, low power consumption and rich peripheral features. It is also supported by a large community and is supported by tools such as "STM32Cube", a widely used development environment.

* ADC:
In electronic boards, ADC (Analog-to-Digital Converter) is a component responsible for converting analog signals to digital signals. Most electronic devices use analog signals to communicate with the world around them. But most microprocessors and digital systems work with digital data. Therefore, ADCs are used to digitally process analog signals or communicate with digital devices.

The ADC takes analog signals from analog signals, usually representing constantly changing physical quantities such as voltage or current, and converts them into digital data that represents them in digital form (numeric data consisting of 0's and 1's). This transformation makes it possible to perform numerical operations, apply digital filters, perform numerical controls, and implement other digital algorithms in microprocessors.

For example, a microprocessor can take the analog signal from a thermometer, convert that signal to digital values ​​using an ADC, and then display this numerical value on a display representing the temperature value or incorporate it into a control algorithm.

The tasks of the ADC in electronic boards include:

Converting Sensor Data to Digital Format: It converts the data from analog sensors (such as temperature, pressure, humidity) into digital values ​​and makes them processable by the microprocessor.
Conversion of Analog Audio to Digital Audio Recordings: In sound cards, analog audio waves are converted into digital audio data and used for digital audio processing and recording.
Storage of Analog Data: The digital memory unit can be used to store analog data in digital data files.
Transmission of Analog Data: ADC provides data transmission to remote devices using digital communication methods, by converting analog data into digital signals.
Digital Control: It makes it possible to use digital control circuits instead of analog control circuits.
Therefore, ADCs provide a bridge between the analog and digital worlds, allowing electronic devices to have a wider range of functionality. The analog-digital conversion process in the electronic world is a very common and important process today. ![](../../../../Downloads/WhatsApp%20Image%202023-07-08%20at%2011.35.18.jpeg)




 



     



