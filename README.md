# LoRa sx1268 Tutorial
## Hello I'm Akhsan

This is my first IoT project using LoRa HAT for Raspberry Pi. In this project, I use Semtech module of LoRa sx1268 assembled by [Waveshare](https://www.waveshare.com
). There are two kind of devices needed, transmitter and receiver. This IoT system works by sending DHT11 sensor data from transmitter to receiver. Receiver must be connected to the internet, so the sensor data can be uploaded to cloud (in this case I use [Antares Platform](https://antares.id)).

In this tutorial I use [Waveshare Documentation](https://www.waveshare.com/w/upload/1/18/SX126X_LoRa_HAT_CODE.zip) and modified it for assembling additional sensor program and connectivity to the Internet Protocol (HTTP).

There are three Python codes above, two of them are transmitter and receiver with almost same program (transmitter has additional line of program to read DHT11 sensor). The other one is used for sx1268 library.

### Note: Under the same frequency, receiver node can send data to transmitter node, similarly as the transmitter node can send data to receiver node. In other word, two nodes must have suitable address each other

## How to operate this system
1. Make sure each node have been attached to Raspberry Pi as microcontroller
2. Connect the sensor cable to Raspberry head-pin (transmitter node) according to the program
3. Make sure all program files have been installed in each Raspberry device
4. Run transmitter and receiver programs on each Raspberry Pi
5. Press 's' button in transmitter's Raspberry device to send sensor data to receiver node
6. Open your [Antares](https://antares.id) project that have been linked to receiver node
7. The DHT11 sensor data can be seen on [Antares](https://antares.id) interface



![Copy of IMG_20211118_175421](https://user-images.githubusercontent.com/57405134/224116148-092b9b73-9080-416b-8d2c-5b548efac409.jpg)
Assembled Components



![IMG_20211118_174842 (1)](https://user-images.githubusercontent.com/57405134/224116198-1c7de213-cedb-4893-abf6-8ec19471278d.jpg)
Components



![IMG_20220116_164616_708 (1)](https://user-images.githubusercontent.com/57405134/224116225-2e00e4f2-d492-44f3-8b07-7f9f1482ea7d.jpg)
Result
