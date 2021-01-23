# GAL16V8 MC14500-LIKE UNIT

See more about MC14500 in [MC14000B INDUSTRIAL CONTROL UNIT HANDBOOK](https://archive.org/details/bitsavers_motorola14alControlUnitHandbook1977_4934745).

This GAL (ATF16V8B...) version of the MC14500 has an original instruction set, but it has some differences:

Data is read from a separate DI input and written to a separate DO output during GAL's clock rise, at the time of instruction execution. This unit does not have usually unused pins RET, FLG0, FLGF (but they are easily to implement each by external single logic gates).

- ICU - GAL14500

- IO - IO chip for GAL14500, provides 4 outputs, 3 inputs and oscillator

- ROMCTL - single chip I2C EEPROM reader and driver for shift register

Use [GALASM](https://github.com/daveho/GALasm) for assemble .pal files.
