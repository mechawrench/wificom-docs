# Parts List

This project is modular, so choose the sections you need. Screen and speaker are optional, but we highly recommend using them as they provide a much easier time with the WiFiCom.

## Minimum base for Pico W on breadboard
- Pi Pico W with headers
- Breadboard: 830 tie points for a full build
- Breadboard jumper wires
    - A kit including some short wires is recommended
    - Or, very short connections can be made using legs cut from extra resistors
- Visible LED: conventionally orange in this project
- 220R resistor
- 1 small pushbutton (tactile switch)

## Screen
- 4-pin SSD1306 128x64 OLED module
    - Note that GND and Vcc are switched on some of these products - check yours carefully!
- 2 more small pushbuttons for 3 in total

## Speaker
- Passive buzzer module with built-in amplifier and 3 pins for Vcc, GND and signal: recommended for breadboarding
- See the schematic for a possible alternative circuit
    - Note: different speakers may need different circuits

## Prong circuit
- Resistors: 1 each of 470K, 100K, 4K7, 1K
- 1nF ceramic capacitor
- Connector to toy e.g. 2 round breadboard jumpers

## IR LED circuit
- (Shared between all IR devices and D-Scanner barcodes)
- IR LED, 940nm or 950nm
    - LEDs with half-angles of 10 and 15 degrees tested and working
    - 30 degrees did not work well with the D-Scanner
- 220R resistor

## Data Link and Fusion Loader
- TSOP4838 IR sensor
- (Also need the IR LED circuit)

## iC/Twin/DigiWindow
- TSMP58000 IR sensor
- (Also need the IR LED circuit)

## Talispod/dam
- 1K2 resistor (1%)
- 3K3 resistor (1%)
- 1nF ceramic capacitor
- Connector to the toy
    - Note: we can't just stick wires into the prongs as with Digimon
    - Craft a connector?
    - Desolder a Talisdam cord, replace with something else, and use the cord with other toys?
    - Custom connectors are in development
