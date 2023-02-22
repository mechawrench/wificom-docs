# Upgrading Software

1. Backup your current files, in particular the following are commonly modified:
    - secrets.py
    - board_config.py
    - config.py (previously digiroms.py)
1. Update CircuitPython if required
1. Put the WiFiCom into drive mode so that the CIRCUITPY drive is writeable
1. Download the latest release from releases page, you'll be looking for a file named "wificom-lib_RELEASEVERSION.zip"
1. Extract the zip and copy the contents into the root of the CIRCUITPY drive
1. Compare contents of your modified files with the new files and make any necessary changes
1. Test that everything works, including connecting to WiFi and sending/receiving DigiRoms
