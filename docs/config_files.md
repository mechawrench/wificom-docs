# Config Files

These files can be edited, and should normally be retained between updates. We may introduce breaking changes to these files that are required to run the software - please check the release notes for any changes to these files.

## secrets.json

(`secrets.py` on v1.x firmware)

Contains credentials for connecting to your WiFi network and the server. Recommended to download from `wificom.dev`, but can also be filled out from `secrets.example.json`.

## config.json

Contains non-secret configuration options.

- "sound_on": `true` or `false`

`config.py` on v1.x firmware: also contained the DigiROMs for the punchbag menu. Check the comments in the file for details.

## digiroms.txt

Contains the DigiROMs for the punchbag menu. Check the comments in the file for details.

## board_config.py

Describes the hardware configuration of the board. You only need to edit this if using an unsupported board or custom circuit layout. Check the comments in the file for details.
