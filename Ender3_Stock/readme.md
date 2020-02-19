# Ender-3-Stock-3DPC

This is an edit of our Ender-3-BLtouch-3DPC firmware.  All changes to restore stock configuration machine behaviour.

## Boards

This firmware has been tested for compatibility with Creality v1.1.4 and v1.1.5 control boards.

## Changes made to recreate a "Stock Config"

### Configuration.h
1) undefined BLTOUCH
2) undefined SERVO0_PIN 27 (required for BL Touch)
3) defined FIX_MOUNTED_PROBE (for Z- limit switch)
4) undefined AUTO_BED_LEVELING_BILINEAR (with BL Touch undefined, we are no longer using auto bed leveling)
5) undefined Z_SAFE_HOMING (causes machine to home at bed center, which is not default stock behaviour)

### Configuration_adv.h
1) undefined BABYSTEPPING (used for BL Touch Z Probe Offset.  Incompatible when BLTOUCH undefined.)

## For Installation Instructions

Please refer to the BL Touch version readme.md file for installation instructions.