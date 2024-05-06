Idea
• ESPHome
	○ https://github.com/syssi/esphome-jk-bms
	○ Need ESP32 that talks to all JK BMSes over bluetooth
	○ This then communicates with HA via esphome

Install

Install ESPHome on a esp32 (through homeassistant ESPHome addon) - this will need to be connected to the computer via usb

Go to discovered devices and add it

Go to ESPHome in the HA sidebar and adopt the newly added device

Each device takes a yaml file (use the edit button to edit this). Get the MAC addresses for each bms using https://github.com/syssi/esphome-jk-bms/blob/main/esp32-ble-scanner.yaml

For reference this is currently:
garage: C8:47:80:09:A3:35
front_cabinet: C8:47:80:09:BA:E8
rear_cabinet: C8:47:80:09:B6:F8

Then use the final yaml: https://github.com/syssi/esphome-jk-bms/blob/main/esp32-ble-example-multiple-devices.yaml
