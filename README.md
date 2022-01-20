# Ender 3 Max to Switchwire Conversion

## Warning
This conversion isn't completed. Please don't use this as-is. If you want to do this conversion, check the modification notes below, but please note that I may have missed something. The list of things to complete are
* Create a rough Ender 3 Max frame to work with
* Move the keyback idler further up on the frame by about 24cm to account for the keyback fully extending/bottoming out.
* Add instructions to drill holes in the Y carriage.
* A mounting method out the sides for the wider virtical extrusions for the enclosure. The overall enclosure will need to be bigger as the virtical extrusions are mounted beside the bottom frame rather than on top of the frame like it is in the Ender 3 and Switchwire.
* The Motor mounts that I'm using should be moved in a little bit before the enclosure can be made as the belts would rub on the enclosure.
* The virtical drag chain part needs to be printed mirrored / sticking out and/or modified in order to fit in the space.

After my build, here are the modifications that I made in the build, but aren't in this branch yet.
* I'm using the motor mounts from https://github.com/VoronDesign/VoronUsers/tree/master/printer_mods/Gizzle/ender-3_(pro)_switchwire
* The [a]_z_chain_lower_mount_generic.stl part needed to be printed mirrored on the x axis to have it go over the edge of the printer.
* The keyback idler needed to be mounted to the outside vslot and about 240mm higher to accomodate the extra virtical space.
* I cut the x axis aluminum extrusion to about 380mm.
* The linear rails that I selected are 2 x 420mm for the Z, 2x400mm for the Y, and 1x350mm for the X.
* I extended the spacer block from the front to 50mm and printed 2 of them for the back grill.
* I used the silicon mod for my bed leveling screws. This meant that the front left screw needed to be cut off.
* The front bed clips were removed, and the back two bed clips were left in place to align the PEI sheet similar to how it would be on a Prusa.

This is a full conversion of the Ender 3 Max to a Voron Switchwire as a fork of boubounokefalos's conversion that he did with [Triano](https://github.com/walttriano). The motivation came from [his awesome original conversion](https://github.com/walttriano/VoronUsers/tree/master/printer_mods/Triano/Ender_3Pro_Switchwire) that was used as a starting point, however almost everything was re-designed from scratch (in order to follow the Voron guidelines and aesthetics more accurately). Another factor that led to this re-design, was the need to be able to enclose this printer in a, visually, pleasant and, structurally, functional way. The ingenious design of 5x MGN12H Linear Rails - 300mm (dual Y axis rail) from Triano was preserved and the printing volume is ~220x220x220.

(For assembly tips regarding some unique parts of this conversion, check the [Wiki](https://github.com/boubounokefalos/Ender_SW/wiki)).

![Home](Images/enclosed.png)
![Home](Images/non_enclosed.png)
![Home](Images/real.png)

## Info

Various parts _can*_ be recycled from the Ender 3 Pro/V2, most important ones are:
- The frame (though a 310mm extrusion is needed for the X. You can chop the original one to length).
- The MeanWell PSU.
- The heatbed assemble.
- The original board.
- XYZ motors (as long as you can pull off the pulleys. An aftermarket 20mm motor is needed for the printhead extruder though).
- All the cables that don't go through the cable-chains (for there, silicone or PTFE cable is adviced).
- 4010 fan for the tool cooling.

*cheaping out in parts can lead into several problems, such as poor printing quality or, even worse, safety hazzard. Keep that in mind and use parts from the official Switchwire BOM.

## Files

- Most of the printed part files needed for this conversion, are included in this git (you will only need to get the Afterburner print files from the [official Switchwire git](https://github.com/VoronDesign/Voron-Switchwire/tree/master/STL/Gantry/XZ_Axis/X_Carriage) ).
- CAD files (.f3d and .STEP) are provided, in order to help the building process, but they also serve as a BOM (in case you need to find proper screw lengths etc).
- DXF files in order to cut your enclosure panels.
- A printer.cfg as a starting point (based off LDO motors and SKR E3 mini V2 board).

## Credits

- Ofc to Triano for his awesome design and all the valuable help, info and support.
- To marcel#0874 for his original idea of the sticky grill endcaps.
- To sdukan#9213 for his valuable help into troubleshooting the Ender 3 V2 differences, electronics (and in general)
- To all of this awesome community of people.
- To Voron design team for all the valuable resources and the solid base.

## Disclaimer

This is a very carefuly designed build.. however mistakes could have been made so by deciding to follow this conversion, you are responsible for any possible damage done to the printer or even yourself. This is serious so keep that in mind.
