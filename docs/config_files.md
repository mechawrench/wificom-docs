# Config Files

These files can be edited, and should normally be retained between updates. We may introduce breaking changes to these files that are required to run the software - please check the release notes for any changes to these files.

## secrets.py

Contains credentials for connecting to your WiFi network and the server. Recommended to download from `wificom.dev`, but can also be filled out from `secrets.example.py`.

## config.py

Contains non-secret configuration options. Check the comments in the file for details.

## board_config.py

Describes the hardware configuration of the board. You only need to edit this if using an unsupported board or custom circuit layout. Check the comments in the file for details.
