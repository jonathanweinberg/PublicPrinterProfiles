G21 ;metric values
G90 ;absolute positioning
M82 ;set extruder to absolute mode

M851 Z0.0

M107 ;start with the fan off

M104 S145 ;Warm up the extruder
M140 S55 ;Warm up the bed

M851 Z0.26

G28

G29

M117 Heating up...

M104 S{material_print_temperature} ; set extruder temp
M140 S{material_bed_temperature} ; set bed temp
M109 S{material_print_temperature} ; wait for extruder temp

M117 PURGING!

G1 Y3.0 F500.0 ; move out of print volume
G1 Z0.25 ; Drop to bed
G1 X60.0 E9 F500.0 ; start purge line
G1 X140.0 E16.5 F500.0 ; finish purge line
G92 E0 ;zero the extruded length again


M205 S0.00 T0.00 B20000 X11.00 Y11.00 Z0.40 E8.00 ; Jerk Settings
M851 Z0.74

M117 Printing...