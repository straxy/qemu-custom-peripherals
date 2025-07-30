# Patches enabling custom QEMU devices from [MistraSolutions blog](https://www.mistrasolutions.com)

This repository holds patches implementing custom QEMU devices for Allwinner-A10/Cubieboard,
described in the
[MistraSolutions blog](https://www.mistrasolutions.com):

- memory-mapped sensor
- I2C temperature sensor
- SPI temperature sensor

The patches are compatible with QEMU v10.0.2.

The I2C and SPI peripherals export a `temperature` property that can be manipulated using QMP,
which is explained in the various
[QMP posts in the MistraSolutions blog](https://www.mistrasolutions.com/tags/qmp/).

The original implementation of those peripherals generated random values of the temperature
every time a read was performed and that implementation is kept in the
[random-values](https://github.com/straxy/qemu-custom-peripherals/tree/random-values)
branch of this repository.
