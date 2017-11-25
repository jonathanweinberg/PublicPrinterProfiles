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

1) [MOSFET Upgrade](https://www.amazon.com/gp/product/B01HEQVQAK/) _**Do THIS UNLESS YOU WANT TO BURN OUT THE MELZI BOARD AND POSSIBLY START A FIRE**_
1) [Flex Couplers (5mm X 8mm X 25mm)](https://www.amazon.com/RepRap-Champion-Flexible-Coupling-printers/dp/B00THZJKPA/) _Overpriced via Amazon, get on AliExpress. I actually don't recommend these anymore, I prefer the "plum couplers"._
1) [Upgraded Y Chassis (RepRap Champions)](https://www.amazon.com/RepRap-Champion-Carriage-Duplicator-Monoprice/dp/B01MUAMRN7/) _**Quite required after a little time as well. Stock tends to warp quickly**_
1) [Upgraded HotBed (RepRap Champions)](https://www.amazon.com/RepRap-Champion-Printer-Aluminum-Adjustment/dp/B019BGAB7K/) _**Gives you a little bit more room since it has recessed screws. This one in particular is nice and flat as well. You can do a 3 point system vs. a 4 point.**_
1) [200 watt silicone heater (RepRap Champions)](https://www.amazon.com/RepRap-Champion-Silicone-Thermistor-Printer/dp/B016CKFZEM/) _**Fancy, heats fast and pretty evenly.**_
1) [Witbot MKS GEN 1.4 (AKA Witbot GEN v1.0 is a MKS GEN 1.4)](https://www.amazon.com/Witbot-Controller-Ramps1-4-Mega2560-DRV8825/dp/B06XD5YT5K/) _**Woo! Nice little RAMPS / Marlin compatible board!**_
1) [Witbot 12864 LCD](https://www.amazon.com/Witbot-Controller-Control-Display-Monitor-Motherboard/dp/B07219RT7R/) _**Perfectly functional, includes an SD Slot, and yes, needs the connectors flipped to be usable.**_
1) [BIQU A4988 Steppers](https://www.amazon.com/gp/product/B01FFFYVV8/) _**OG steppers work fiiiiiiiiiine.**_

1) [BLTouch Smart](https://www.amazon.com/BLTouch-Leveling-Sensor-Premium-Printer/dp/B076PS71B8/)

   * [BLTouch Mount Used](https://www.thingiverse.com/thing:2335175)

1) [Micro Swiss All Metal Hotend with SLOTTED Cooling Block for Wanhao i3](https://www.amazon.com/Micro-Hotend-SLOTTED-Cooling-Wanhao/dp/B01E1HANLS) _**Yes. It works. No more worrying about PTFE Tubing. At all. Install is easy, yet tricky.**_
1) [Micro Swiss CNC Machined Lever and Extruder Plate for Wanhao i3 (Full Kit)](https://www.amazon.com/Micro-Swiss-Machined-Extruder-Wanhao/dp/B06WVB6CYD/) _**Mostly just pretty, but also functional. Nothing truly innovative about the design. Would have like to have seen a bit more engineering in it, making an actual pivot point versus a screw. But no wondering if it's gonna wear out slightly and send your filament out the side when you change.**_
1) [Micro Swiss nozzle for All Metal Hotend Kit ONLY A2 Hardened Steel .4mm](https://www.amazon.com/Micro-Swiss-nozzle-Hotend-Hardened/dp/B01LOYTH86/) _**Reminder that the one that comes with the Micro Swiss kit is a brass "hardening coated" nozzle. Abrasive filaments like Glow In The Dark, or Aluminum fill'd ones will eat it slower than a straight brass nozzle, but it'll still happen. This should last longer.**_

1) 4mm Borosilicate Glass 219mm x 219mm (RepRap Champions) _**Link to Come**_
1) 3mm Borosilicate Glass 213mm x 200mm (Signstek) _**Link to Come**_
1) 1/4" Plain Window Glass 213mm x 213mm (Generic) _**More info to come**_
1) GizmoDorks PEI Sheet _**Link to Come**_
1) Anycubic Ultrabase _**Link to Come**_

## Helpful links

* Marlin Configuration Tools

  * [Marlin firmware configurator (Thingiverse)](https://www.thingiverse.com/thing:2403436)
  * [Marlin firmware configurator (GitHub kaJes/marlin-config)](https://github.com/akaJes/marlin-config)
  * [Marlin3DprinterTool](http://marlin3dprintertool.se) _**Very neat .NET app**_
  * [Ginge's reimplemented from scratch and memory of the Daid's marlin builder web app.](https://github.com/ginge/marlin-builder) _**Old, probably not something to use**_



#### Software Side

* Marlin Configuration

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