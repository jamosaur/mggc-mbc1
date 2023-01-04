# MGGC X jamo_mods MBC1 carts

There are 2 versions of the MBC1 cart. The original one only supports up to 512kb roms (unless you feel like doing some hacky bodges), V2 has full support for 2mb roms.

## BOM

| Reference | Description | Footprint | Extra |
| --- | --- | --- | --- |
| R1 | 10kΩ | 0603 | |
| C1, C2, C3 | 100nF | 0603 | |
| U1 | AM29F016 | TSSOP-48 | |
| U2 | BA6129 | SOIC-8 | harvest from donor |
| U4 | MBC1 | SOIC-24 | harvest from donor |
| U5 | SRAM | SOIC-28 | harvest from donor |

## Bodge fix for V1

By hooking up 2 wires you can get full 2mb support on a v1 board.

| MBC PIN | FLASH PIN | |
| --- | --- | --- |
| 6 | 3 | 3rd pin from top right of flash |
| 7 | 46 | 3rd pin from the bottom right of flash |


## Version differences

### V1

These boards can be identified by the two solder jumpers at the bottom right of the cart.

**Only `AUD` should be bridged**, using `WR` is not advised.

### V2

These boards don't have any solder jumpers and are produced in purple.
