# Printrbot Metal Plus Single Extruder Independent Dual Z Axis
#### Z Axis alignment using G34 Auto Align

This firmware requires testing. Use M119 command to verify the Z axis endstop functionality before homing.

This firmware requires the SKR 1.4 Turbo with 5x TMC2209 Stepper Drivers.
Z1 (Left Stepper Motor) plugs into Z Port) 
Z2 (Right Stepper Motor plugs into E2 Port)

Command:
G28 ;home all
G34 ;z axis auto align 

https://marlinfw.org/docs/gcode/G034.html

This configuration provides automatic Z axis calibration using the Z axis inductive probe.
The bed is probed in two known locations using the G34 command, the firmware automatically adjusts the XZ gantry to be level with the bed.

This firmware assumed stock configuration
M92 X80 Y80 Z2020 E94.5

If you are using a 4-start lead screw, make sure to enter this gcode or adjust via LCD.
M92 Z400

Stock V1 or V2 Printrbot Extruder
E94.5

Aftermarket 11.95mm Diameter Extruder
E102

Save Using M500
Download Firmware.bin file and copy to the root directory of the micro sd card provided with the controller.