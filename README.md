# ONIX FMC Host Board
This card provies a host interface for serialized headstages and miniscopes, as
well as general purpose analog and digital IO. It is a VITA-57.1
compliant module that uses high pin-count FMC connector. In combination with a
base FPGA board (e.g. [Numato Lab
Nereid](https://numato.com/product/nereid-kintex-7-pci-express-fpga-development-board),
it provides host PC communication for the following:

- Two deserailizers for any multifunction headstage conforming to the ONIX
  serialization protocol
- 12x 16-bit, +/-10V analog outputs or inputs. Direction selected via analog
  switch controllable over the FMC connector. Analog inputs are separated into
  2 simultaneously sampled 6-channel banks. 
- Analog output are always looped back using the analog inputs.
- 3x high speed LVDS input pairs
- 2x high speed LVDS outputs pairs
- 2x high speed, arbitrary logic-level, singled-ended Hi-Z or 50-ohm clock inputs
- 1x high speed single ended, 50-ohm clock output
- 4x MLVDS input or output trigger lines

![fmc-host revision 1.4 on Numato Lab Nereid](./resources/host-board_edited.jpg)
