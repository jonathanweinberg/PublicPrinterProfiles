M502 ; Reset EEPROM
M501 ; Restore EEPROM

M104 S145 ;Warm up the extruder
M140 S40 ;Warm up the bed

G21 ;metric values
G90 ;absolute positioning
M82 ;set extruder to absolute mode

M107 ;start with the fan off

G28 ; home all axes
G29 ; AutoBedLevel

M851 Z-0.38 ; Z-Probe Settings
;M92 X79.55 Y79.6 Z394.71 E106.35 ; Step Settings
M92 X79.25 Y79.3 Z394.71 E100.35

;M205 S0.00 T0.00 B20000 X6.00 Y6.00 Z0.40 E6.00 ; Jerk Settings
M205 S0.00 T0.00 B20000 X8.00 Y8.00 Z0.40 E6.00

;G1 Z15.0 F{travel_speed} ;move the platform down 15mm
;G92 E0 ;zero the extruded length
;G1 F200 E6 ;extrude 6 mm of feed stock
;G92 E0 ;zero the extruded length again
;G1 F{travel_speed}

M117 Heating up...

M104 S{material_print_temperature} ; set extruder temp
M140 S{material_bed_temperature} ; set bed temp
M109 S{material_print_temperature} ; wait for extruder temp

M117 PURGING!

G0 Z0.25 ; Drop to bed
G1 Y3.0 F500.0 ; move out of print volume
G1 X60.0 E9 F500.0 ; start purge line
G1 X100.0 E12.5 F500.0 ; finish purge line
G92 E0 ;zero the extruded length again

M117 Printing...