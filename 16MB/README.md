# GVP-Compatible 64-Pin 16MB SIMM

*Warning: Beta Version! This has not been fabricated nor tested, build at your own risk*

This is a 16MB (4Mx32) SIMM design for certain GVP accelerator cards. It's
64-pin but follows the proprietary GVP pinout.

Since this is a beta version, fab files have not been generated. If you have
the expertise to get the files, load them in KiCad, and generate the fab
files, you're probably OK with doing some experimentation to get these working.

Board dimensions are 3.85 x 0.925 inches. It is a 4 layer board. When
ordering, **please specify a board thickness of 1.2mm!** This ensures that
it will fit in the SIMM slot. Again, to emphasize: most quick-turn board
services use 1.6mm thick boards by default which will not fit in a SIMM
slot. Be sure to select 1.2mm!

## DRAM Chips

KM44C4000AS-6, K4F1704110-FC60, or equivalent 60ns fast page mode memory
chips (16 megabit).

Be sure that the memory chip you select has a 12-bit row address and a 10-bit
column address -- sometimes known as "4K refresh" because a full refresh
must access all 4096 row addresses. It must also operate at 5V.

## Bypass Capacitors

Use eight 0603 capacitors with a value of at least 0.22uF. Ensure the voltage
rating is 10V or higher. Do not use 6.3V rated capacitors since they are too
close to the rail voltage of 5V.

## Assembly Notes

Since the chips are fairly close together, I recommend ordering the boards
with a solder stencil and using solder paste with a reflow process (or
hot plate) to solder the components.

## License

This project is licensed under the CERN Open Hardware License Version 2 - Permissive.
