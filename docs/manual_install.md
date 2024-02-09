# Manual Installation

Most users should use `wificom-update-tool` as described in [Device Setup](device_setup.md) instead!

## CircuitPython

`wificom-lib` runs on CircuitPython 8.x. Check the CHANGELOG for the exact version tested with each release.

## Release Zips

[wificom-lib releases](https://github.com/mechawrench/wificom-lib/releases) bundle all required libraries, and are compiled to `mpy` format for faster startup.

## Instructions

1. Backup your current files, in particular the following are commonly modified:
    - secrets.py
    - board_config.py
    - config.py (previously digiroms.py)
1. Update CircuitPython if required
1. Put the WiFiCom into drive mode so that the CIRCUITPY drive is writeable
1. Download the latest release from releases page, you'll be looking for a file named "wificom-lib_RELEASEVERSION.zip" or "wificom-lib_RELEASEVERSION_picow.zip"
1. Extract the zip and copy the contents into the root of the CIRCUITPY drive
1. If this a new installation, add secrets.py
1. Otherwise, compare contents of your modified files with the new files and make any necessary changes
1. Test that everything works, including connecting to WiFi and sending/receiving DigiRoms

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
