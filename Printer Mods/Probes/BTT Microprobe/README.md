# Positron v3.2 - BTT Microprobe Mod
This mod allows for a Microprobe to be mounted to the Toolhead.

For Wiring reference, please see [LDO's Positron Hardware Repo](https://github.com/MotorDynamicsLab/PositronHardware/tree/master/PositronV3.2).

This mod uses some existing hardware, and mounts to the Toolhead's Heatsink. This part is very thin to allow for maximum clearance between the toolhead and the extruder. Please test your setup to ensure there is no collision.

The Servo cable is plugged into the SERVOS pins on the MCU - GPIO29

The Probe cable is plugged into the TH0 pins on the MCU - GPIO27
> Note - TH0 / GPIO27 is unused in stock configuration.

# Required Hardware
- 2x m2.5x10 for Probe Mount
- 12x 3x2mm Magnets
- 4x M2.5x6 BHCS (Included in Positron Kit)
- JST PH 2Pin Female + JST PH 3Pin Female to JST GH 5Pin Female Connector (**not** included with BTT Microprobe)

# Installation Instructions
1. Glue 6x 3x2mm Magnets into the `Probe_Heatsink_Mount`
2. Glue 6x 3x2mm Magnets into the `BTT_Microprobe Probe Harness`
3. Ensure the Magnet polarities match to allow the two parts to magnetically mount.
4. On the underside of the toolhead, remove the 4x M2.5x6 BHCS screws holding the heatsink to the bottom plate.
5. Using the screws you just removed, mount the `Probe_Heatsink_Mount` to the underside of the bottom plate, using the same holes as before.
6. Mount the BTT Microprobe to the `BTT_Microprobe Probe Harness`
7. Test and make sure the two components can magnetically couple, and decouple.

# Recommended Print Settings

 - We recommend printing all parts in ABS or ASA
 - [We're copying Voron's homework;](https://docs.vorondesign.com/sourcing.html#print-settings)
    - Layer height: 0.2mm
    - Extrusion width: 0.4mm
    - Infill percentage: 40%
    - Infill type: grid, gyroid, honeycomb, triangle, or cubic
    - Wall count: 4
    - Solid top/bottom layers: 5
    - Supports: You should be able to get away with none, but you may need a few as there are a few major overhangs.

ABS or ASA is the recommended filament for most parts, PLA and PETG can be used for many accent pieces, but please only do so at your own discretion.

# Questions or Comments
Please feel free to join our [Discord](https://discord.gg/mGDkYZtyNY) to help with any feedback. We appreciate any and all feedback that can help us better improve our designs.
