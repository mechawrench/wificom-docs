# Supported Boards

`wificom-lib` is designed for boards with RP2040+WiFi.

## Supported Boards
- Raspberry Pi Pico W - RECOMMENDED OPTION
- Arduino Nano Connect
- RP2040 with AirLift co-processor module
    - Pi Pico is the only tested board so far but others should work as well
    - Pi Pico does not have enough pins to enable all WiFiCom features

## Unsupported Boards
- RP2040 Challenger with WiFi Chip
    - Issues with SSL with onboard chip; doesn't allow for secure requests
- RP2040 Challenger with WiFi/BLE Chip
    - Issues with SSL with onboard chip; doesn't allow for secure requests
