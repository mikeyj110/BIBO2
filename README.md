# About
This is a hub for things that I've found helpful when working with the BIBO Touch 2 3D Printer.

-------------------------------------------------
## Links
  - [BIBO 3D Printer Facebook Group](https://www.facebook.com/groups/192868111095711)
    - Facebook user group for BIBO 3D printer users
  - [Makerbase: MKS SGEN_L V1](https://github.com/makerbase-mks/SGEN_L)
    - Official Github for the __SGEN 32-bit__ Equivalent board.  The standard board is the `MKS GEN_L V1` which is Arduino based.
    - Though this is NOT the standard version of the board for BIBO, it does have a lot of useful information.
  - [MKS Tool](https://baizhongyun.cn/home/mkstoolview)
    - Tool to help build custom firmware.
    
-------------------------------------------------

## Marlin Firmware Settings (MKS GEN_L V1 - Standard Board)
  - Core - Arduino
  - Motherboard - BOARD_MKS_GEN_L
  - Name - MKS Gen L
  - Pins - pins_MKS_GEN_L.h

## Marlin Firmware Builds (MKS SGEN_L V1 - 32-Bit Board)
  - Settings for build in Platformio.ini
    ```
    [platformio]
    src_dir      = Marlin
    boards_dir   = buildroot/share/PlatformIO/boards
    default_envs = LPC1768
    include_dir  = Marlin
    ```
  - Motherboard settings for Configuration.h
    ```
    #ifndef MOTHERBOARD
      #define  MOTHERBOARD BOARD_MKS_SGEN_L   // BOARD_MKS_SGEN_L
    #endif
    ```