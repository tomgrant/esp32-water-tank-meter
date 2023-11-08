# esp32-water-tank-meter
Water meter using an ESP32 and sonar sensor to be used in Home Assistant

Note that the configuration of your yaml file may differ, especially around keys like `esphome:` and `esp32:`

## Hardware

The hardware used in this project is a standard ESP-32 development board, a waterproof enclosure and an HC-SR04P Ultrasonic Module. This project is mains powered, and the polling time on the sensor is short. If you choose to make this a solar/battery-powered project, you will need to change this.

Drill two holes in the bottom of the enclosure for the two ultrasonic sensors to stick out of and seal around them to ensure moisture can't work its way into the enclosure. Preferably with silicon or hot glue.

