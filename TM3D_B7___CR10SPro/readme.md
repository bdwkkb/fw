# TinyMachines3D (TM3D) CR-10S Pro (v1) Firmware
aka InsanityAutomation

This is a backup of a very reliable version of firmware for the CR-10S Pro (v1) machines.  It has been superceded by the DW5 releases.

This backup includes both a stock (capacitive sensor) and a BL Touch probe version of the software plus the screen files.  The screen files are the same.  But if the machine has been converted to a BL Touch probe, please use the BL Touch version.

For the best results we recommend adding "G29" on the line following "G28" in your slicer start gcode.  This will tell your machine to probe the bed and use the results to compensate.  This is preferable to the M420 (use pre-saved mesh) that is in the stock profiles (at least in Cura.) 
