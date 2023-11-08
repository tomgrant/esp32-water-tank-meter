# esp32-water-tank-meter
Water meter using an ESP32 and sonar sensor to be used in Home Assistant

Note that the configuration of you yaml file may differ, especially around keys like `esphome:` and `esp32:`

## Hardware

The hardware used in this project is a standard ESP-32 development board, a waterproof enclosure and a HC-SR04P Ultrasonic Module. This this project is mains powered, the polling time on the sensor is short. If you choose to make this a solar/battery powered project, you will need to change this.

Simply drill two holes in the bottom of the enclosure for the two ultrasonic sensors to stick out of and seal around them to ensure moisture can't work it's way into the enclosure. Preferably with silicon or hot glue.