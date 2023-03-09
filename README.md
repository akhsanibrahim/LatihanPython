# LoRa sx1268 Tutorial
## Hello I'm Akhsan

This is my first IoT project using LoRa HAT for Raspberry Pi. In this project, I use Semtech module of LoRa sx1268 assembled by [Waveshare](https://www.waveshare.com
). There are two kind of devices needed, transmitter and receiver. The IoT system works by sending HC-SR04 sensor data from transmitter to receiver. Receiver must be connected to the internet, so the sensor data can be uploaded to cloud (in this case I use [Antares Platform](https://antares.id)).

In this tutorial I use [Waveshare Documentation](https://www.waveshare.com/w/upload/1/18/SX126X_LoRa_HAT_CODE.zip) and modified it for assembling additional sensor program and connectivity to the Internet Protocol (HTTP).

There are three code above, two of them are transmitter and receiver with almost same program (transmitter has additional line of program to read HC-SR04 sensor). The other one is used for sx1268 library.

### Note: under the same frequency, receiver node can send data to transmitter node, similarly as the transmitter node can send data to receiver node. Otherwise two nodes must have suitable address each other

## How to operate this system
1. Make sure each node have been attached to Raspberry Pi as microcontroller
2. Connect the sensor cable to Raspberry head-pin (transmitter node) according to the program
3. Make sure all program files have been installed in each Raspberry device
4. Run transmitter and receiver programs on each Raspberry Pi
5. Press 's' button in transmitter's Raspberry device to send sensor data to receiver node
6. Open your [Antares](https://antares.id) project that have been linked to receiver node
7. The HC-SR04 sensor data can be seen on [Antares](https://antares.id) interface

