# Pico-ESP32-BLE
This project allows you to communicate between a Raspberry Pi Pico W and ESP32 using BLE. I will accompany this project with a Medium article soon.

## Code

Inside the `pico_esp32` folder here are the files:

* `pico_central.py`: This is used for the Pico W as it will act as the central device. This code looks for the Peripheral and then connects to it.
* `esp32_per.py`: This is used for the ESP32 as it will act as the Peripheral. This code will connect to the Central Device and then send data to it.
* `uuids.json`: This json file contains the UUIDs for the service and characteristic. This should be copied to both devices because without it, neither will work correctly.
