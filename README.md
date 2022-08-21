# Epson Printhead Driver

This is a driver for Epson piezo inkjet printheads, based heavily on Joyce G. Kwan's prior work. It provides a PMOD interface for use with FPGA development boards such as the [iCEBreaker](https://1bitsquared.com/collections/fpga/products/icebreaker). The goal is to enable use of cheap and widespread Epson printheads in DIY projects.

These printheads require an analog signal to actuate the piezos. This signal is actually fairly high voltage/power. It peaks around 33V, and if you're activating all nozzles, you can be supplying over 3A to the printhead. Therefore, we need a DAC with an amplifier capable of supplying that much power. This makes up the bulk of the project.

## Tested on

* Epson XP4105

## References

* [Joyce Kwan's Master's Thesis](https://dspace.mit.edu/bitstream/handle/1721.1/85435/870681346-MIT.pdf?sequence=2_1)