# Patches enabling custom QEMU devices from [MistraSolutions blog](https://www.mistrasolutions.com)

This repository holds patches implementing custom QEMU devices for Allwinner-A10/Cubieboard, described in the
[MistraSolutions blog](https://www.mistrasolutions.com):

- memory-mapped sensor
- I2C temperature sensor
- SPI temperature sensor

The patches are compatible with QEMU v9.1.0, but in order to have SPI temperature sensor the Allwinner A10 patches from
the QEMU master branch should be manually applied.
