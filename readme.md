# Project  S3 Trio64V+ VLB  aka  ET4000 & ARK1000VL hunter
"Making a Concurrent for Creative 3D Blaster VLB"
A spinoff of  failed old project for 486 platform: S3 Trio64V+ with 2MB DRAM.
It is just a  Replica of  STB Powergraph 64V VLB with addition of few hardware for ViRGE (86C325).
Full history ->  https://www.vogons.org/viewtopic.php?f=63&t=76647

![pictures](https://github.com/matt1187/765VL/blob/main/picture/765VL_000.jpg)

# PCB Revision History  (attention, two PCB type )
- 325VL-000 initial draft
- 765VL-000 spinoff of 325VL-000 included bug fixing (DDC interface, config strap ), removed discrete adress decoder
- 325VL-001 added SAUP2 delaying, added s3d logo

# Feartures
- S3 Trio64V+ video chipset 
- one of  fastest video card for VESA local bus platform. (only ARK 1000VL is faster in DOS, on edge!)
- 2 MB DRAM
- 135 MHz integrated RAMDAC
- rock solid  40 MHz bus-clock with zero wait-state
- Win 3.1, Win9x, Win NT 3.51 & 4 driver available
- cheap Trio64V+ PCI card as component-donor.
  
# Issues 
- 50 MHz bus-clock -> RAMDAC isn't capable to handle of high clock (graphic artifact in DOOM). Except this issues, is video card stable.
- some motherboard (SIS 496/497, UM8810  ) doesn't work with zero waitstate of 765VL.
- some issues with zero waitstate (win 3.1 artificial, crash) VLB interface buggy ?
- small SOJ-40 footprint requires good solder skill. 
- no official S3 VBE 2.0  with linear framebuffer support. (it requires modification of S3VBE318.EXE)
Quote of mkarcher "As S3VBE20 is not "free/open source software", I don't have a license to modify it, to run modified versions, and certainly not to distribute modified versions, though. If you want to take the legal risk yourself, get S3VBE/Core 2.0 version 3.18, understand that the terms of use explicitly state that the license for using, copying and distributing only applies "if you don't modify the files in this package in any way", so you certainly wouldn't undo the LZEXE compression, and patch the byte at offset 0x2d2f from 0x75 to 0xEB."

# note
- it would work with S3 ViRGE (86C325), but major bug on VLB interface and no driver for ViRGE VLB is available.
- all component with  followed ID is optional (R50-55, U50, J3, D50-57, RP5, RP6)
It has debug function and isn't required for working of card.

 

# Pictures

# Bill of material

- [![](https://github.com/matt1187/765VL/blob/main/gerber/765VL000.csv')](#bom)
- [![Config strap (R100-R150 ), here a picture of config strap resistor ](https://github.com/matt1187/765VL/blob/main/pictures/765VL_configstrap.jpg)

# driver & ROM 
- [![fastest ROM for Trio64V+ VLB, 0 WS](https://github.com/matt1187/765VL/blob/main/rom/highspeed_ROM.zip)]
- [![Powergraph 64V ROM, 1 WS](https://github.com/matt1187/765VL/blob/main/rom/PG64V12.zip)]

- [![Windows 3.1 driver](https://github.com/matt1187/765VL/blob/main/driver/STB_Powergraph64V_drivers_WIN31_from_STB_p64v212h.zip)]
- [![Windows 95 driver](https://github.com/matt1187/765VL/blob/main/driver/STB_Powergraph64V_drivers_WIN95_from_STB_p64V124h.zip)]
- [![Windows NT 3.51 driver](https://github.com/matt1187/765VL/blob/main/driver/STB_Powergraph64V_drivers_WINNT4_from_S3.zip)]
- [![Windows NT 4 driver](https://github.com/matt1187/765VL/blob/main/driver/STB_Powergraph64V_drivers_WINNT351_from_S3.zip)]

#note
all component with  followed ID is optional (R50-55, U50, J3, D50-57, RP5, RP6)
It has debug function and isn't required for working of card.




# License
The project is free for non-commercial reproduction. Do not sell it on Ebay or other platforms for profit. Do not make a closed source derivative. Share your experiences and ideas with the community.

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License][cc-by-nc-sa].

[![CC BY-NC-SA 4.0][cc-by-nc-sa-image]][cc-by-nc-sa]

[cc-by-nc-sa]: http://creativecommons.org/licenses/by-nc-sa/4.0/
[cc-by-nc-sa-image]: https://licensebuttons.net/l/by-nc-sa/4.0/88x31.png