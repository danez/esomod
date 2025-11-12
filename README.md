# esoMOD

An easy to use replacement board for irrigation systems by esotec GmbH. Makes
these irrigation systems smart, allows them to be added to HomeAssistant, and
adds advanced functionality.

![PCB_PCB_esoMOD_2025-09-12](https://github.com/user-attachments/assets/23eb68b5-01f0-4c37-9067-3749699b49c1)

## Compatibility

All the here mentioned products use the same control device, so the assumption
is that they are all compatible. If you have one of the not tested products feel
free to send me a picture of the CircuitBoard inside the product and I can
verify if it will work.

| Name                                                                                                         | Compatible | Tested |
| ------------------------------------------------------------------------------------------------------------ | ---------- | ------ |
| [WaterDrops Professional](https://www.solarversand.de/solar-bewaesserungsset-waterdrops-professional/)       | ✅         | ❌     |
| [WaterSprinkle Professional](https://www.solarversand.de/solar-bewaesserungsset-watersprinkle-professional/) | ✅         | ✅     |
| [WaterSpray Professional](https://www.solarversand.de/solar-bewaesserungsset-waterspray-professional/)       | ✅         | ❌     |

## Changelog

#### 2.2

- Remove UART completely as unused
- Add some more vias

#### 2.1

Rotate the resistors for the battery voltage divider to have cleaner traces

#### 2.0

- Fix resistor value from 51Ohm to 51kOhm
- Fix sensor to ESP connections it was reversed
- Fix sensitivity of button by adding a capacitor, it was way to high
- Remove reset button, as main switch can be used as reset
- Remove boot button as not needed to flash
- Change UART to be to small simple pads to save some space

#### 1.1

Minor small fixes

#### 1.0

Initial version

## Boards

I ordered 5 Boards from JLCPCB already partly assembled and currently try to get
the software all up and running. I will only use one, so if you are interessted
shoot me an email or open and issue.

![PXL_20250718_093847694](https://github.com/user-attachments/assets/04bb3d56-a7cd-44dd-8d21-5a836abe3687)

This is the working v1.0 version I use with some fixes for the wiring.
