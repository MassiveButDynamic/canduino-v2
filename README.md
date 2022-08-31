# CANdunio v2

Here you can find a tutorial how to get started with your CANduino `v2`. Please make sure that you really use the `v2`, because on `v3` the CS_Pin was `CS_Pin 8`!

## Getting started

The following library must be installed before use: https://github.com/autowp/arduino-mcp2515/archive/master.zip

If your CANduino is at the end of the CANbus chain, it is mandatory to connect the CAN_T jumper (next to the CAN connector)!

## Important parameters

So that the mcp2515 can be addressed it is important to set the following parameters:
```
MCP2515 mcp2515(10);
mcp2515.setBitrate("Your Bitrate", MCP_8MHZ);
```

## Example Code

In the `examples` folder you will find two code examples with which you have the possibility to `send` and `receive` CAN messages.

## Troubleshooting

If you have the `CANduino v3 with ATmega168PA` the following board manager URL must be inserted in the programming environment (Arduino IDE). The bootloader is preinstalled: https://mcudude.github.io/MiniCore/package_MCUdude_MiniCore_index.json

Please use our instructions for v3 which you can find here: https://github.com/MassiveButDynamic/canduino-v3 or for v3.1 https://github.com/MassiveButDynamic/canduino-v3.1

## Pinout

Here you can find a pinout of the CANduino v2:
![Pinout](/Pinout-CANduinov2.jpg)
