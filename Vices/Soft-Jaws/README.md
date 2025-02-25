# Vice Jaw Operation 1 Overview

## Tool Changes and Operations

### Tool 9 - 3 Flute DLC (3mm)
- **RPM**: 15,000
- **Feed Rate**: 2,000 mm/min
- **Operation**: Adaptive clearing
- **Coolant**: Mist (M7)
- **Variable Spindle Speed Control**: Enabled (P4000 V200)

### Tool 3 - Single Flute (12mm)
- **RPM**: 20,000
- **Feed Rate**: 1,000 mm/min
- **Operation**: Adaptive clearing
- **Coolant**: Mist (M7)
- **Variable Spindle Speed Control**: Enabled (P4000 V200)

### Tool 2 - Double Flute 17mm Ball
- **RPM**: 20,000
- **Feed Rate**: 960 mm/min
- **Operation**: Scallop
- **Coolant**: Mist (M7)
- **Variable Spindle Speed Control**: Enabled (P4000 V200)

### Tool 6 - Chamfer Mill (3mm)
- **RPM**: 20,000  
- **Feed Rate**: 2,000 mm/min
- **Operation**: 2D Chamfer
- **Coolant**: Mist (M7)
- **Variable Spindle Speed Control**: Enabled (P4000 V200)

## Process Overview
1. Initial setup and probing
   - Probes reference surface
   - Uses WCS 1 (G54)
   - Probes origin in current WCS
   - Enables rotation compensation

2. Main Adaptive Operation (Tool 9)
   - Multiple adaptive clearing passes
   - Complex contour following
   - Multiple Z-level operations

3. Secondary Adaptive Operations (Tool 3 & Tool 2)
   - Additional adaptive clearing passes
   - Complex contour following
   - Multiple Z-level operations

4. Chamfer Operation (Tool 6)
   - 2D chamfering around the perimeter
   - Single pass at -3mm depth

## Safety Features
- Firmware version check (v0.5.0-rc1)
- Tool details passed to firmware
- Spindle acceleration monitoring
- Variable speed control for vibration reduction
- Coolant control
- Automatic parking between operations

## Notes
- File includes extensive safety checks and spindle controls
- Uses RRF firmware-specific features
- Includes automatic probing and work coordinate system management
- Multiple parking and tool change operations
- Comprehensive coolant and spindle speed management

# Vice Jaw Operation 2 Overview

## Tool Changes and Operations

### Tool 1 - 3 Flute DLC (3mm)
- **RPM**: 15,000
- **Feed Rate**: 2,000 mm/min
- **Operation**: Adaptive clearing
- **Coolant**: Mist (M7)
- **Variable Spindle Speed Control**: Enabled (P4000 V200)

### Tool 6 - Chamfer Mill (3mm)
- **RPM**: 20,000
- **Feed Rate**: 2,000 mm/min
- **Plunge Feed**: 333.3 mm/min
- **Operation**: 2D Chamfer
- **Coolant**: Mist (M7)
- **Variable Spindle Speed Control**: Enabled (P4000 V200)

## Process Overview
1. Initial setup and probing
   - Probes reference surface
   - Uses WCS 1 (G54)
   - Probes origin in current WCS
   - Enables rotation compensation

2. Main Adaptive Operation (Tool 1)
   - Multiple adaptive clearing passes
   - Complex contour following
   - Multiple Z-level operations at -3.9mm, -8.4mm, -17.7mm depths

3. Chamfer Operation (Tool 6)
   - 2D chamfering around the perimeter
   - Single pass at -10.449mm depth
   - Includes both external and internal feature chamfering

## Safety Features
- Firmware version check (v0.5.0-rc1)
- Tool details passed to firmware
- Spindle acceleration monitoring
- Variable speed control for vibration reduction
- Coolant control
- Automatic parking between operations

## Notes
- Operation 2 focuses on the opposite side of the vice jaw
- Includes deeper cutting operations than Operation 1
- Multiple Z-level passes for material removal
- Comprehensive safety checks and spindle controls
- Uses RRF firmware-specific features
- Includes automatic probing and work coordinate system management