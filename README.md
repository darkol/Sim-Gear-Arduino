# Sim Gear Library for Arduino

Based on the **Sim Racing Library** for Arduino ATMega32U4 by Dave Madison to extend the supported hardware connected as USB HID game controller device.

The library is intended for usage with raw hardware interfaces, replacing original controllers legacy interface electronics.

Examples of adapters converting legacy interfaces to USB:
* [GamePort Adapter](https://github.com/necroware/gameport-adapter) - Arduino ATMega32U4 based GamePort adapter supporting analog and several digital protocols
* [Arduino NES/SNES USB](https://github.com/mooware/arduino-nes-snes-usb) - Arduino ATMega32U4 based NES/SNES gamepad adapter
* ...


## Sim Racing Library for Arduino
[![arduino-library-badge](https://www.ardu-badge.com/badge/Sim%20Racing%20Library.svg?)](https://www.ardu-badge.com/Sim%20Racing%20Library) [![Build Status](https://github.com/dmadison/Sim-Racing-Arduino/workflows/build/badge.svg)](https://github.com/dmadison/Sim-Racing-Arduino/actions/workflows/ci.yml) [![Documentation](https://img.shields.io/badge/Docs-Doxygen-blue.svg)](http://dmadison.github.io/Sim-Racing-Arduino/docs/index.html)
[![LGPL license](https://img.shields.io/badge/License-LGPL-orange.svg)](https://github.com/dmadison/Sim-Racing-Arduino/blob/master/LICENSE)

The [Sim Racing Library](https://github.com/dmadison/Sim-Racing-Arduino/) is an Arduino library for interfacing sim racing equipment such as pedals and gear shifters with Arduino development boards.

Author: Dave Madison

## Getting Started

Install the library using either [the .zip file from the latest release](https://github.com/darkol/Sim-Gear-Arduino/releases/latest/) or **TODO** by searching for "Sim Gear" in the libraries manager of the Arduino IDE. [See the Arduino documentation on how to install libraries for more information.](https://docs.arduino.cc/software/ide-v1/tutorials/installing-libraries)

**TODO** Read the documentation ([https://dmadison.github.io/Sim-Racing-Arduino/docs/md_pages_2supported__devices.html](https://dmadison.github.io/Sim-Racing-Arduino/docs/index.html)) to check if your device is supported by the library. Follow the wiring instructions on the device page to connect your device to the Arduino.

Run one of the library examples in the Arduino IDE by going to `File -> Examples -> Sim Gear Library`. For all peripherals, call `begin()` to initialize the class and `update()` to refresh with new data.

Upload example to the Arduino board and device should ne recognized as Game Controller upon next USB connection.

On Windows press Windows key + `joy.cpl` to open the control panel with listed game controller devices and do initial Calibration of the newly connected device.


## Supported Devices

### Generic Devices
* [Two pedal peripherals (gas + brake)](https://dmadison.github.io/Sim-Racing-Arduino/docs/class_sim_racing_1_1_two_pedals.html)
* [Three pedal peripherals (gas, brake, clutch)](https://dmadison.github.io/Sim-Racing-Arduino/docs/class_sim_racing_1_1_three_pedals.html)
* [Analog shifters](https://dmadison.github.io/Sim-Racing-Arduino/docs/class_sim_racing_1_1_analog_shifter.html)
* [Analog handbrakes](https://dmadison.github.io/Sim-Racing-Arduino/docs/class_sim_racing_1_1_handbrake.html)
**TODO**
* Joysticks
* PAS pedal sensor

### Commercial Devices
* [Logitech Two Pedal Peripheral (Gas, Brake)](http://dmadison.github.io/Sim-Racing-Arduino/docs/logitech_pedals.html)
* [Logitech Three Pedal Peripheral (Gas, Brake, Clutch)](http://dmadison.github.io/Sim-Racing-Arduino/docs/logitech_pedals.html)
* [Logitech Driving Force Shifter](http://dmadison.github.io/Sim-Racing-Arduino/docs/logitech_shifter.html)
**TODO**
* Thrustmaster [T500RS](https://support.thrustmaster.com/en/product/t500rs-en/)/[T3PA-PRO Pedals](https://support.thrustmaster.com/en/product/t3papro-en/)
* Logitech Wingman Extreme Digital

## Adapters

### Sim Racing Adapters

Open source shields are available to connect the [Logitech Three Pedal Peripheral](http://dmadison.github.io/Sim-Racing-Arduino/docs/logitech_pedals.html) and the [Logitech Driving Force Shifter](http://dmadison.github.io/Sim-Racing-Arduino/docs/logitech_shifter.html) to a [SparkFun Pro Micro](https://github.com/sparkfun/Pro_Micro). The design comes with a 3D printable case and custom board files so that the adapter appears with a custom identity and "Sim Racing" name over USB. You can use these shields to build an inexpensive USB HID adapter.

You can find all of the necessary files in [the project repository](https://github.com/dmadison/Sim-Racing-Shields).

## License

This library is licensed under the terms of the [GNU Lesser General Public License (LGPL)](https://www.gnu.org/licenses/lgpl.html), either version 3 of the License, or (at your option) any later version. See the [LICENSE](https://github.com/dmadison/Sim-Racing-Arduino/blob/master/LICENSE) file for more information.
