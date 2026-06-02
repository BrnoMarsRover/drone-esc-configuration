# Actual setup

- Motors: Holybro X500 V2 Brushless Motor 2216 920kv
- ESCs: Holybro Tekko32 F4 45A ESC AM32 ESC 2S-6S (pdf in repo)
- Propellers: Holybro S500 V2 1045 propeller

# ESC configuration

- [Configurator](https://am32.ca/configurator)
- [How to connect PC to ESC](https://wiki.am32.ca/guides/Arduino-PC-Link.html), I flashed the linked code (Arduino_AM32_pin3Link) to arduino NANO, no custom connector is needed (PWM -> D3, GND -> GND)
- Binary file of my settings is in tekko32_config

# Communication protocol

- DShot300

## Author
Martin Kriz