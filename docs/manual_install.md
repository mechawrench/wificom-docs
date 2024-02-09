# Manual Installation

Most users should use `wificom-update-tool` as described in [Device Setup](device_setup.md) instead!

## CircuitPython

`wificom-lib` runs on CircuitPython 8.x. Check the [CHANGELOG](https://github.com/mechawrench/wificom-lib/blob/main/CHANGELOG.md) for the exact version tested with each release.

- [Raspberry Pi Pico W](https://adafruit-circuit-python.s3.amazonaws.com/index.html?prefix=bin/raspberry_pi_pico_w/) (WiFiCom)
- [Raspberry Pi Pico](https://adafruit-circuit-python.s3.amazonaws.com/index.html?prefix=bin/raspberry_pi_pico/) (P-Com)
- [Xiao RP2040](https://adafruit-circuit-python.s3.amazonaws.com/index.html?prefix=bin/seeeduino_xiao_rp2040/) (P-Com)

## Release Zips

[wificom-lib releases](https://github.com/mechawrench/wificom-lib/releases) bundle all required libraries, and are compiled to `mpy` format for faster startup.

## Manual Installation

1. Install CircuitPython, checking board and version as above
1. Download the latest release from releases page, you'll be looking for a file named "wificom-lib_RELEASEVERSION.zip" or "wificom-lib_RELEASEVERSION_picow.zip"
1. Extract the zip
1. If you are using an unsupported board or custom circuit layout, modify "board_config.py" so the pinouts match your board
1. Copy the files into the root of the CIRCUITPY drive
1. Add secrets.py, either by modifying secrets.example.py, or you can get a prefilled version on wificom.dev
1. Safely remove / eject the CIRCUITPY drive from your computer
1. Cold reboot the WiFiCom (remove and restore power)

## Manual Update

1. Backup your current files, in particular the following are commonly modified:
    - secrets.py
    - board_config.py
    - config.py (previously digiroms.py)
1. Update CircuitPython if required
1. Put the WiFiCom into drive mode so that the CIRCUITPY drive is writeable
1. Download the latest release from releases page, named as above
1. Extract the zip
1. Compare contents of your modified files with the new files and make any necessary changes
1. Copy the files into the root of the CIRCUITPY drive
1. Safely remove / eject the CIRCUITPY drive from your computer
1. Reboot the WiFiCom using one of the options indicated

## Libraries

These are included in the release zip. If installing manually, check `sources.json` for versions. In particular, `adafruit_minimqtt` is likely to break if a different version is used from the one specified.

- [dmcomm-python](https://github.com/dmcomm/dmcomm-python)
- [Adafruit CircuitPython MiniMQTT](https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT)
- [Adafruit CircuitPython Library Bundle](https://github.com/adafruit/Adafruit_CircuitPython_Bundle)
    - adafruit_bus_device
    - adafruit_display_text
    - adafruit_esp32spi
    - adafruit_displayio_ssd1306
    - adafruit_requests

## Server

wificom.dev is open-source. The code is available at:

- [wificom-webapp](https://github.com/mechawrench/wificom-webapp/)
- [wificom-mosquitto-docker](https://github.com/mechawrench/wificom-mosquitto-docker/)
