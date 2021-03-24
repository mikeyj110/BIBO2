//Makerbase: MKS SGEN_L V1
https://github.com/makerbase-mks/SGEN_L

//MKS Tool
https://baizhongyun.cn/home/mkstoolview

//  Platformio.ini
[platformio]
src_dir      = Marlin
boards_dir   = buildroot/share/PlatformIO/boards
default_envs = LPC1768
include_dir  = Marlin

//  Configuration.h
#ifndef MOTHERBOARD
  #define  MOTHERBOARD BOARD_MKS_SGEN_L   // BOARD_MKS_SGEN_L
#endif