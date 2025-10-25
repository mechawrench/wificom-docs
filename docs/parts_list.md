# Parts List

This project is modular, so choose the sections you need.

## Shipping from USA
- Most parts are available from DigiKey
    - [Shared Cart](https://www.digikey.com/short/745zd0nz)
    - Parts in this cart are labelled BASE/PRONG/IR/LEGENDZ - you can delete unneeded items before purchase
- [Pi Pico W with pre-soldered headers (Amazon)](https://www.amazon.com/Pico-Raspberry-Pre-Soldered-Dual-core-Processor/dp/B0BK9W4H2Q/)
    - Can be found cheaper if you're able to solder the headers on
- [Screen (Amazon)](https://www.amazon.com/HiLetgo-Serial-128X64-Display-Color/dp/B06XRBTBTB/)
- [Speaker module (Amazon)](https://www.amazon.com/Tegg-Passive-Speaker-Arduino-Raspberry/dp/B07PRTMF89/)
- [TSMP58000 sensor (eBay)](https://www.ebay.com/itm/285265795138) - for iC/Twin infrared
- Xanthos has Legendz connectors for sale ([Discord](buy_premade.md))

## General Parts Info

### WiFiCom base
- Pi Pico W with headers
- Breadboard: 830 tie points for a full build
- Breadboard jumper wires
    - A kit including some short wires is recommended
    - Or, very short connections can be made using legs cut from extra resistors
- Visible LED: conventionally orange in this project
- 220R resistor
- 3 small pushbuttons (tactile switch)
- Screen: 4-pin SSD1306 128x64 OLED module
    - Note that GND and Vcc are switched on some of these products - check yours carefully!

### Speaker
- Passive buzzer module with built-in amplifier and 3 pins for Vcc, GND and signal: recommended for breadboarding
- See the schematic for a possible alternative circuit
    - Note: different speakers may need different circuits

### Prong circuit
- Resistors: 1 each of 470K, 100K, 6K8, 1K
- 1nF ceramic capacitor
- Connector to toy e.g. 2 round breadboard jumpers

### IR LED circuit
- (Shared between all IR devices and D-Scanner barcodes)
- IR LED, 940nm or 950nm
    - OFL-5102 or LTE-4208 works well
- 220R resistor

### Data Link and Fusion Loader
- TSOP4838 IR sensor
    - Vishay brand recommended - other brands may have issues with Data Link
- (Also need the IR LED circuit)

## iC/Twin/DigiWindow
- TSMP58000 IR sensor
    - Discontinued - possible replacements are under investigation
- (Also need the IR LED circuit)

### Talispod/dam
- 1K2 resistor (1%)
- 3K3 resistor (1%)
- 1nF ceramic capacitor
- Connector to the toy
    - Note: we can't just stick wires into the prongs as with Digimon
    - Buy a premade connector?
    - Craft a connector?
    - Desolder a Talisdam cord, replace with something else, and use the cord with other toys?
