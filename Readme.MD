# Printer Configs

This is a copy of the configuration for Marlin 1.1.5 that I am currently using for my `WanHao \ PowerSpec \ Maker Select i3`.

There is no guarantee on this working well, or safely for you. I take no part in any liability, nor do I claim any stake in the [Marlin project](https://github.com/MarlinFirmware/Marlin/releases).

### You will want to take a look primarily at changes in these locations

* [Configuration.h](PowerSpec-WanHao_i3/Marlin-1.1.5_Release/Marlin/Configuration.h)

* [Configuration_adv.h](PowerSpec-WanHao_i3/Marlin-1.1.5_Release/Marlin/Configuration_adv.h)

* [Slicer / M503 Settings](PowerSpec-WanHao_i3/Current_Settings/)

  * Look in the numbered subfolders....

### Warnings!

 *DO NOT JUST BLINDLY USE THIS WITH A BLTouch. Your Z Probe Offset is likely different.*

*DO NOT EXPECT THIS TO WORK IN GENERAL! Sanity check everything.*

## Current WanHao i3 Configuration

My current printer configuration / changes - not all are relevant:
1) MOSFET Upgrade
1) Flex Couplers (5mm X 8mm X 25mm)
1) Upgraded Y Chassis (RepRap Champions)
1) Upgraded HotBed (RepRap Champions)
1) 4mm Borosilicate Glass 219mm x 219mm (RepRap Champions)
1) 3mm Borosilicate Glass 213mm x 200mm (Signstek)
1) 200 watt silicone heater (RepRap Champions)
1) MicroSwiss Full Metal Hot End
1) Witbot MKS GEN 1.4 (AKA Witbot GEN v1.0)
1) Witbot 12864 LCD
1) BIQU A4988 Steppers
1) BLTouch Smart

   * [BLTouch Mount Used](https://www.thingiverse.com/thing:2335175)

## Helpful links

#### Software Side

* Marlin Configurator

  * Thanks Max!
  * [Thingiverse](https://www.thingiverse.com/thing:2403436)
  * [GitHub](https://github.com/akaJes/marlin-config)
  * [Instructables](http://www.instructables.com/id/Marlin-config/)

#### Hardware Side

* [Stepper Driver Direction Identification](https://3dprinting.stackexchange.com/questions/3456/motor-driver-chip-install-direction/3654#3654)

* [MKS GEN - RepRap Wiki](http://reprap.org/wiki/MKS_GEN)

* [A4988 Stepper Motor Driver Carrier](https://www.pololu.com/product/1182)

* [Board Replacement Options (RAMPS, RADDS, Clone Mini)](https://3dprinterwiki.info/wiki/wanhao-duplicator-i3/di3-advanced-mods/board-replacement-options/)

* [3D Printer Filament Diameter Sensing : Assembled](https://www.tindie.com/products/JasonKits/3d-printer-filament-diameter-sensing--assembled-/)

## Big thanks to...

1) Jonathon Hale

    * Jonathon helped me out a ton with a base configuration, and working through my pesky axis directionality issues. Thank you!

      * [Facebook](https://www.facebook.com/jon012198)

      * [GitHub](https://github.com/jon012198)

1) David Thomas

    * Endless providing of links to resources to understand use of the BLTouch, bed preparation, and some truly excellent example prints.

1) Max DiOrio

    * Tons of great links and direction, discussion of Marlin settings at all hours.