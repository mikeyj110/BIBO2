# About
This is a hub for things that I've found helpful when working with the BIBO Touch 2 3D Printer.

-------------------------------------------------
## Makerbase: MKS SGEN_L V1
Official Github for the standard board.
    https://github.com/makerbase-mks/SGEN_L

## MKS Tool
Tool to help build custom firmware.
    https://baizhongyun.cn/home/mkstoolview

-------------------------------------------------
## Marlin Firmware Builds
Settings for build in Platformio.ini
    [platformio]
    src_dir      = Marlin
    boards_dir   = buildroot/share/PlatformIO/boards
    default_envs = LPC1768
    include_dir  = Marlin
Motherboard settings for Configuration.h
    #ifndef MOTHERBOARD
      #define  MOTHERBOARD BOARD_MKS_SGEN_L   // BOARD_MKS_SGEN_L
    #endif