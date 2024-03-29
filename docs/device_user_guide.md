# Device User Guide

## Units with Screen

The UI has a small screen and 3 buttons.

### Buttons
- Button A: select menu options
- Button B: activate selected option
- Button C: cancel/return (needs to be held for several seconds when device is busy)

### Menu options
- WiFi: Connect to WiFi and MQTT and await instructions from the server
- Serial: Act as a normal serial com unit
- Punchbag: Communicate with the toys in a standalone mode (you can edit `config.py` to change the available options in this submenu)
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
- LED OFF with short blinks indicates a managed failure, follow the instructions on the screen, or on screenless units press the button to restart
- LED OFF indicates failure, please restart your device
- During startup, see below

## Button Usage During Startup
This is the only way to select a mode on units without a screen.

### WiFiCom devices
- To use "WiFiCom mode (with drive read-only)", do not press the button. On units without a screen, this is mostly equivalent to picking "WiFi" from the menu.
- To use "WiFiCom mode (with full drive access)", also known as "Dev mode", hold the C button until the LED comes on, then release.
- To use "Serial Only mode", hold the C button until the LED comes on, and keep holding until the LED goes dim or off. This is mostly equivalent to picking "serial" from the menu.

### P-Com devices
- To use "Serial Mode", do not press the button. This is mostly equivalent to picking "Serial" from the menu.
- To use "Dev Mode", hold the C button until the LED comes on (does not matter when the button is released). If you do not have a LED, hold the C button until the CIRCUITPY drive appears.
