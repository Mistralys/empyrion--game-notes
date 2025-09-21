# Emyprion Game Notes

Notes for the PC game "Empyrion Galactic Survival"

## Small Vessels (SV)

### Warp Capability

Small vessels can only warp within the same solar system. Trying to warp to another system fails with the message "0.0LY range". Inter-system warp is only possible with a capital vessel (CV).

## Power management

### Solar Power

**Yellow lights**: Current amount of sunlight hitting the panels  
**Green lights**: Theoretical maximum production

> Green lights should always be at 4, yellow ones should be at 4 at noon when the sun is highest.

- Build your base near the equator to get the most sunlight.
- Choose a planet / location with a clean atmosphere (no toxic gases or the like).
- Choose a planet not too far away from the sun.

## Editing game files

### Increased solar panel efficiency

1. Open the file `Content/Configuration/BlocksConfig.ecf`.
2. Search for `SolarPanelBlocks`.
3. Adjust the value of `SolarPanelEfficiency`.

Look for `SolarPanelSmallBlocks` if you also wish to adjust the small panels.

> NOTE: Double-check where you're placing your base - see [Solar Power](#solar-power).

### Increase the solar panel build limit

1. Open the file `Content/Configuration/BlocksConfig.ecf`.
2. Search for `SolarPanelBlocks`.
3. Increase the value of `MaxCount`.
4. Search for `SolarPanelSlope`.
5. Increase the value of `MaxCount` to the same value.

### Increased Teleporter range

Teleporter Block names:

- TeleporterBA
- TeleporerBAT1
- TeleporterBAEpic
- TeleporterBAEvent
- TeleporterCV

1. Open the file `Content/Configuration/BlocksConfig.ecf`.
2. Search for the teleporter entries.
3. Look for the `RangeLY` property, add it if it does not exist.
5. Set the value to use (I have gone as high as 9000). 

> As the comments in the file show, a value of `0` restricts teleportation to the current system.

### Increased Warp Drive range

1. Open the file `Content/Configuration/BlocksConfig.ecf`.
2. Search for `RangeLY`.
3. This will find both warp drive blocks and teleporter blocks.
4. Adjust the value of `RangeLY`.
