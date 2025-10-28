# Chain
The Chain is a mix of CAN, LIN, USB and I2C that connects all [Cogs](https://github.com/PedalPirat/Cogs) of the [PedalPirat](https://github.com/PedalPirat/PedalPirat) Ecosystem

## Overview
A smart bike has a lot of components in different places, using different methods of communication and in general don't like to talk to components of other manufacturers.

Maybe I want to use Shimano Di2 Levers and Brakes with SRAM AXS shifters. [Do what you want because a pirate is free](https://youtu.be/i8ju_10NkGY?si=5lvISrumFXBw_ymA)

The Chain is the sum of all connections (and connectors) which are needed for the project.

### Protocols
As we are dealing with a wild mix of devices with different connectors, quite a few protocols need to be suppoted.
### [ANT+](https://www.thisisant.com/developer/ant-plus/ant-antplus-defined/)
ANT+ is a quite old mesh network that is used a lot in smart cycling and other sport products.
For example SRAM AXS is basically just a branded name for ANT+.

Shimano Di2 (wireless) also uses ANT but is a custom implementation which has already been [reverse engineered](https://titanlab.co/reverse-engineering-shimano-di2/)
### BTLE
More and more product (sadly) ditch ANT+ and use [Bluetooth Low Energy](https://www.nordicsemi.com/Products/Wireless/Bluetooth-Low-Energy) instead.
### [CAN](https://www.csselectronics.com/pages/can-bus-simple-intro-tutorial)
Controller Area Network (CAN) is a Bus which is used a lot in automotive and robotics. It's a masterless Bus which enables communication between up to 256 Nodes.

Like Cars, components for E-Bikes use them to communicate with each other, the main computer with the motor, the battery or the speed sensor or the Rohloff E-14.

#### [LIN](https://www.csselectronics.com/pages/lin-bus-protocol-intro-basics)
The Local Interconnect Network (LIN) Bus is often used together with CAN and used for example for light controllers in cars (and also our Lights, because we also want cool animations).
#### USB
Cameras and other stuff, m'kay?
#### I2C
### Power
Sensors, Shifters etc need power which is also provided via the connection.

## Data

## [ThingSet](https://thingset.io/)
