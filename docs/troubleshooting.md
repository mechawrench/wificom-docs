# Troubleshooting

## Via Serial

Please use [NacaBattle Serial Console](https://battle.nacatech.es/nt/console) for interfacing with serial on your WiFiCom. To see messages that appear on WiFiCom startup, click inside the DigiROM input box and ensure it is empty, press Control-C to stop the program, then Control-D to start it from the beginning.

[Code with Mu](https://codewith.mu/) is another option. Choose CircuitPython mode and click the Serial/REPL button. To see messages that appear on WiFiCom startup, press Control-C in the Serial/REPL area to stop the program, then Control-D to start it from the beginning.

GNU Screen also works and may be preinstalled on Mac/Linux systems.

Arduino IDE is not recommended because it cannot send the Control-C and Control-D characters.

## Log Files

If your WiFiCom crashes, note the 3-digit number on the screen, press the button indicated to reboot, then check the CIRCUITPY drive for `wificom_log.txt`. There should be an entry matching the number you noted earlier.
