# IMPORTANT FOR THIS FOLDER

These are the printed parts for the original / OLD Extruder v1.  The [LDO Assembly Guide](https://ldomotion.com/guides/1---positron-v32---extruder) currently shows the instructions for this.

We do strongly suggest instead using the v2 Extruder if possible.  It is substantially more reliable and performant.

An assembly guide for the Extruder v2 is in progress, but you may find it helpful to use the [Positron3D CAD Viewer](https://cad.positron3d.com/?model=Positron_v3.2.2) and expand into the Extruder_v2 to see how it goes together.

## BOM
All needed parts are included with the LDO Positron Kit (there are plenty of extra fasteners):
- M2x10 Self Tapping Screw (Quantity: 2)
    - Used to attach the Z Endstop Switch to the `extruder_v2_main_body`)
- M3x25 BHCS (Quantity: 3)
    - 1x goes from the bottom through `extruder_v2_bottom_plate` and `extruder_v2_main_body` into a M3x5x4 Heatset Insert in `extruder_v2_motor_plate`.
    - 2x go through the bottom of `extruder_v2_main_body` into the LDO Pancake Stepper.
- M3x8 BHCS (2x)
    - 2x go through the bottom of `extruder_v2_bottom_plate` into M3x5x4 Heatset Inserts in `extruder_v2_main_body_*`.
- M3x5x4 Heatset Insert (Quantity: 4)
    - 1x goes into the bottom of `extruder_v2_motor_plate` (see above).
    - 2x go into the bottom of `extruder_v2_main_body_*` (see above).
    - 1x goes into the side of `extruder_v2_guidler`.
- M4 Hex Nut (Quantity: 2)
- M4x10 BHCS (Quantity: 2)
- EITHER: M3x35 SHCS or M3x35 BHCS OR the silver M3 Thumbscrew (see note below) (Quantity: 1)
    - This goes through the spring, through the washer, and into the front of `extruder_v2_main_body` and into the M3x5x4 Heatset Insert on `extruder_v2_guidler` as the tensioning mechanism.
- Extruder BMG Spring
- Washer

## Extruder Main Body Notes!
There are two versions for this part:  

Option A)
If you would like to use a M3x35 SHCS (Socket Head) or M3x35 BHCS (Button Head) as the tension fastener, use the `extruder_v2_main_body_m3x35.stl`.  Once tension is set, it generally never needs adjustment, so the smaller form factor is nice.

Option B)
If you would like to use the Silver M3 Thumbscrew supplied in the LDO Kit (originally used with the old Extruder V1), use `extruder_v2_main_body_m3thumbscrew.stl`.

Print information for the new Extruder v2 is found below:

## Colors and Naming
You will see two options;
1. If there is a `[a]` at the start of the filename, this denotes it can be printed with an accent color
    - This is a secondary, often complimentary color, and will help your build pop.
2. If there is no prefix at the start of the filename, this denotes it can be printed with the main color
    - This is the majority of the parts of the build.

Of course, these are just color coordination suggestions, please experiment and have fun!
