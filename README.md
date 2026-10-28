# Home Assistant RF + IR Bridge

A wireless module for adding RF and IR capabilities to Home Assistant. Built on an ESP32-S2. Uses the MQTT protocol.

## Firmware

A template ESPHome firmware is included in the `esphome` dir.

For the CC1101 with custom RF protocol decoders (e.g. manually decoding timings on async serial), ESPHome is too fat.
My [rf-bridge-cc1101](https://github.com/grimsteel/rf-bridge-cc1101) firmware is a dedicated ESP-IDF firmware which uses an RMT encoder instead. This uses MQTT.

## Case

[Onshape Design](https://cad.onshape.com/documents/3fa20c9ad7bfb09f7d235099/w/0402c86a1dfdebba9d6406ce/e/ae3f75737fe19659bf3606c5?renderMode=0&uiState=6ae175f6d8fa074995ccf596)

The case can be 3d-printed in two parts: the base and the cover.

The base:
* Has two spots for heatsets
* Slots for front/side IR leds, photoresistor, and USB port.
* Optional slot for side CC1101

The cover:
* Slots into the base
* Has a wall hook

<img width="600" alt="Case render" src="https://github.com/user-attachments/assets/654bc0db-b100-47f7-8ab9-c2f53732dbeb" />


## PCB

* Front: includes pin sockets for two CC1101 modules. (allows for RX/TX on multiple freqs if needed)
* Back: space for two 6mm buttons, two IR leds, and one IR receiver.

![image](https://github.com/user-attachments/assets/1217d0b5-bb71-4ceb-9051-dba940389f5e)
