# Emyprion Game Notes

Notes for the PC game "Empyrion Galactic Survival"

## Small Vessels (SV)

### Warp Capability

Small vessels can only warp within the same solar system. Trying to warp to another system fails with the message "0.0LY range". Inter-system warp is only possible with a capital vessel (CV).

## Editing game files

### Increased solar panel efficiency

1. Open the file `Content/Configuration/BlocksConfig.ecf`.
2. Search for `SolarPanelBlocks`.
3. Increase the value of `SolarPanelEfficiency`.

Look for `SolarPanelSmallBlocks` if you also wish to adjust the small panels.

> NOTE: Check the output of the solar system's sun. If the planet only receives very little sunlight, increasing the efficiency will have little effect.

### Increase the solar panel build limit

1. Open the file `Content/Configuration/BlocksConfig.ecf`.
2. Search for `SolarPanelBlocks`.
3. Increase the value of `MaxCount`.
