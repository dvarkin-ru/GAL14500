# GAL16V8 MC14500-LIKE UNIT

See more about MC14500 in [MC14000B INDUSTRIAL CONTROL UNIT HANDBOOK](https://archive.org/details/bitsavers_motorola14alControlUnitHandbook1977_4934745).

This GAL (ATF16V8B...) version of the MC14500 has an original instruction set, but it has some differences in working with peripherals:

The contents of the PC must be incremented after GAL's Clock fall, data is read from a separate DI input and written to a separate DO output during GAL's clock rise, at the time of instruction execution. PC and MC14500 reset must be synchronous during clocking. Logically NOR clock and reset for L to H clocked PC clock, as an option. This unit does not have usually unused pins RET, FLG0, FLGF (but they are easily to implement each by external single logic gates). W pin must be logically ANDed with Clock pin for Write strobe.

Use [GALASM](https://github.com/daveho/GALasm) for assemble project from .pal file.
