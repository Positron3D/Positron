# PLEASE READ ME
This is stock configs for the Positron, but you need to double check things!

# Things to Check
## Z_Endstop
First, in `Printer.cfg`, check your `endstop_pin`;
```python
## Choose only one of the following lines for z homing ##
# endstop_pin: probe:z_virtual_endstop  ; virtual endstop probe 
endstop_pin: gpio3                      ; microswitch
```
By default, it is set to `gpio3` as we are moving to a microswitch configuration. If you have not installed a Z_Endstop, please comment this line out and uncomment `probe:z_virtual_endstop`;
```python
## Choose only one of the following lines for z homing ##
endstop_pin: probe:z_virtual_endstop  ; virtual endstop probe 
#endstop_pin: gpio3                      ; microswitch
```
This will re-enable the IR Sensor.

## Driver Strengths - Sensorless Homing
We have a middle of the road average for this, but it will vary between printers, so please check this.
In your klipper console, run;

`SET_TMC_FIELD STEPPER=stepper_x FIELD=SGTHRS VALUE=60`

This will likely cause your printer to home Z too early, the higher the number in `VALUE` the higher the sensitivity of the sensorless homing. Re-run this command with a slightly lower value (we reccomend reducing by increments of 5), until your X axis is reliably homing.
- Note; you may need to move the bed down a bit every time, as it is likely to move up each time you attempt this.

Once you are happy with your X homing, and it isn't skipping when it reaches 0 on the X axis, take that value and go into `sensorless_homing_pv3.cfg` and set the following;
```python
[tmc2209 stepper_x]
diag_pin: ^gpio16
driver_SGTHRS: -> UPDATE THIS VALUE <-
```

Repeat this process for the Y axis using;

`SET_TMC_FIELD STEPPER=stepper_y FIELD=SGTHRS VALUE=60`

and once again, find the correct value for your Y Axis, and update the following;
```python
[tmc2209 stepper_y]
diag_pin: ^gpio25
driver_SGTHRS: -> UPDATE THIS VALUE <-
```