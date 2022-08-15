# flash-tasmota

This script attempts to make flashing the Tasmota firmware to a Sonoff S31 as
easy as possible. The inspiration for this script comes from https://www.adventurousway.com/blog/sonoff-s31

### Dependencies

- Serial cable. I use a FTDI TTL-232R-3V3
- [esptool.py](https://github.com/espressif/esptool)
- [tasmota.bin](https://github.com/arendst/Tasmota/releases), there are many to
    choose from, but you want `tasmota.bin` from the current releases
- `flash-tasmota` from this repository

### Usage

Attempts will be made to automatically detect your serial device for writing. If
detection fails, you'll be prompted to set the `SERIAL` environment variable for
an explicit device.

The script will look for `tasmota.bin` in the current directory. If the firmware
is not found, you'll be prompted to set the `TASMOTA` environment variable for
the explicit firmware file.

### Note

This process does not back up the stock firmware.
