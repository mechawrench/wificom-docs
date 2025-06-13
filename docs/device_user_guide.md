# Device User Guide

## WiFiCom UI

WiFiCom has a small screen and 3 buttons.

### Buttons
- Button A: select menu options
- Button B: activate selected option
- Button C: cancel/return (needs to be held for several seconds when device is busy)

### Menu options
- WiFi: Connect to WiFi and MQTT and await instructions from the server
- Serial: Act as a normal serial com unit
- Punchbag: Communicate with the toys in a standalone mode (you can edit `digiroms.txt` to change the available options in this submenu)
- Settings:
    - Version Info: Show the version info
    - Sound: Toggle sound ON/OFF.
    - Drive: Make the CIRCUITPY drive writeable so you can edit configuration or update firmware
    - UF2 Bootloader: Activate the RPI-RP2 drive for updating CircuitPython

## LED Indicator
- Raspberry Pi Pico W: external LED on GP10
- Raspberry Pi Pico: on-board green LED
- Seeed Xiao RP2040: external LED on A3

### LED Meanings
- Blinking indicates connecting to WiFi and MQTT
- Solid (dimmed) LED indicates connected and no errors
- Solid (bright) LED indicates waiting for Digimon/Legendz device during real-time battle
- LED OFF with short blinks indicates a managed failure, follow the instructions on the screen
- LED OFF indicates failure, please restart your device

## Button Usage During Startup
- To enter "Dev mode", connect the USB while holding the C button (the single separate button on P-Coms) and keep holding until the CIRCUITPY drive appears
    - This means the main program is running with the CIRCUITPY drive writeable
    - On WiFiComs, mainly used for dev, but sometimes useful for recovering from incorrect files
    - On P-Coms, used to edit configuration or update firmware
- For WiFiComs with v1.x firmware, the above enters serial mode. To enter "Dev mode", start the same way but release the button promptly when the LED comes on
