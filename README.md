# esp32-water-tank-meter
Water meter using an ESP32 and sonar sensor to be used in Home Assistant

Note that the configuration of your yaml file may differ, especially around keys like `esphome:` and `esp32:`

## Hardware

The hardware used in this project is a standard ESP-32 development board, a waterproof enclosure and an HC-SR04P Ultrasonic Module. This project is mains powered, and the polling time on the sensor is short. If you choose to make this a solar/battery-powered project, you will need to change this.

Drill two holes in the bottom of the enclosure for the two ultrasonic sensors to stick out of and seal around them to ensure moisture can't work its way into the enclosure. Preferably with silicon or hot glue.

![20230930_214056](https://github.com/tomgrant/esp32-water-tank-meter/assets/1542257/c5d60e83-8692-4289-925f-a37f27af4f55)

## Home Assistant
For displaying the water tank level in Home Assistant I went with a [bar card](https://github.com/custom-cards/bar-card)https://github.com/custom-cards/bar-card through HACS. Note this is no longer maintained, but works great for this application. 

![image](https://github.com/tomgrant/esp32-water-tank-meter/assets/1542257/1041d195-2814-4330-ac42-1434123969ec)

The exposed sensors in home assistant are:
 - Water level as total Litres remaining
 - Water level percentage
 - Distance Sensor - The current distance to the top of the water  
