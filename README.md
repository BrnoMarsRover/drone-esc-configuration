# Actual setup

- Motors: Holybro X500 V2 Brushless Motor 2216 920kv
- ESCs: Holybro Tekko32 F4 45A ESC AM32 ESC 2S-6S (pdf in repo)
- Propellers: Holybro S500 V2 1045 propeller

# ESC configuration

- [Configurator](https://am32.ca/configurator)
- [How to connect PC to ESC](https://wiki.am32.ca/guides/Arduino-PC-Link.html), I flashed the linked code (Arduino_AM32_pin3Link) to arduino NANO, no custom connector is needed (PWM -> D3, GND -> GND)
- Binary file of my settings is in tekko32_config

**AM32 ESC Settings**

**BaseTune:** Bootloader PIN: PA2, Version: 1, MCU: F421 (EEPROM v2)
**Firmware:** TEKKO32_F421 v2.17

**Motor Settings:**
- Protocol: Auto
- Reversed: Yes | 3D mode: No
- Stuck rotor protection: ✓ | Stall protection: ✓
- Use hall sensors: No | 30ms interval telemetry: No
- Variable PWM: ✓ | Complementary PWM: ✓ | Auto timing advance: ✓
- Timing advance: 15° | Startup power: 90%
- Motor KV: 940 | Motor poles: 14
- Beeper volume: 5 | PWM Frequency: 24kHz–48kHz

**Limits:**
- Low voltage cut off: No | Temperature limit: 100 | Current limit: 26
- Low voltage cut off threshold: 300

**Sinusoidal Startup:**
- Sinusoidal startup: Yes | Sine Mode Range: 20 | Sine Mode Power: 8

**Brake:**
- Brake on stop: No | Car type reverse braking: No
- Brake strength: 10 | Running brake level: 10 | Active brake power: 255% duty cycle

**Servo Settings:**
- Low threshold: 1006 | High threshold: 2006 | Neutral: 1502 | Dead band: 50

# Communication protocol

- DShot300

## Author
Martin Kriz