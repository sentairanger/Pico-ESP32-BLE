# Pico-ESP32-BLE
This project allows you to communicate between a Raspberry Pi Pico W and ESP32 using BLE. I will accompany this project with a [Medium](https://medium.com/p/16ff26bde913) article soon.

## Code

Inside the `pico_esp32` folder here are the files:

* `pico_central.py`: This is used for the Pico W as it will act as the central device. This code looks for the Peripheral and then connects to it.
* `esp32_per.py`: This is used for the ESP32 as it will act as the Peripheral. This code will connect to the Central Device and then send data to it.
* `uuids.json`: This json file contains the UUIDs for the service and characteristic. This should be copied to both devices because without it, neither will work correctly.

Inside the `pico_esp32_dual` folder are these files:
* `pico_central_dual.py`: This code sends data from the Pico to the ESP32 and receives data from the ESP32 to the Pico.
* `esp32_per_dual.py`: This code sends data from the ESP32 to the Pico and receives data from the Pico to the ESP32.
* `uuids.json`: Same file as before.

![image](https://github.com/sentairanger/Pico-ESP32-BLE/blob/main/pico-esp32_bb.jpg)
