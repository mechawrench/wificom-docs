# Device Setup

## First Steps

1. [Build your WiFiCom](diy_build.md) or [buy a premade unit](buy_premade.md)
1. For DIY units or if you need to update firmware:
    - Download [wificom-update-tool](https://github.com/mechawrench/wificom-update-tool/releases) and follow the [instructions](https://github.com/mechawrench/wificom-update-tool/blob/main/README.md)
    - If you have a premade, you can skip this step (your unit will have current firmware as of time of sale)

## Obtain secrets

1. Create an account on [wificom.dev](https://wificom.dev/)
1. Go to the [WiFiComs](https://wificom.dev/wifi-devices) section on the website
1. Click "New WiFiCom", enter a device name, then click "Create"
1. On your newly created WiFiCom page, scroll down to the "Credentials Download" section
1. Recommended: Use the "Local Only Configurator" and enter your WiFi network information (this is not shared with wificom.dev). Otherwise you will need to add it to the file after downloading.

## Copy secrets to your WiFiCom

1. Connect your WiFiCom to a computer using a data cable
1. Put your WiFiCom into Drive Mode
    - Up to v1.1.0: found in the main menu
    - v1.2.0+: found in the Settings menu
1. Copy the secrets file into the drive named CIRCUITPY
1. Safely remove / eject the CIRCUITPY drive from your computer
1. Reboot your WiFiCom
    - Up to v1.1.0: choose an option from the menu
    - v1.2.0+: hold C to reboot
