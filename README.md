Additional setup

Printer.cfg
> [include sudrien-bigtreetech-manta-e3ez.cfg]


Cura >> settings >> printer >> manage printers >> machine settings

Start G-code
> START_PRINT BED_TEMP={material_bed_temperature_layer_0} EXTRUDER_TEMP={material_print_temperature_layer_0}

End G-code
> END_PRINT

Cura Plugins
- Calibration shapes
- Mesh tools (slow, maybe not for long)
- Moonraker connection (stack of error messages if printer isn't on)

Cura custom profile changes
- retraction length: 1mm (can grind filament beyond gripability otherwise)


![E3EZ ports](./BIGTREETECH%20Manta%20E3EZ%20V1.0-Interface.jpg)


- One 24v MFAN is pointed at X & Y drivers. Either one will do.
- CB1 requires a heatsink, but seems to be ok without a fan.
- FAN0 is red & black - and needs a connector crimped.
- FAN1 is blue & yellow
- HE0 is the woven red wires
- Get some ferrules on non-jst wires for mechanical soundness and less fire

TODO:

- FAN2 hooked to a filter (24V? buck converter?)
- RGB can power a pure white 24V LCD strip?
