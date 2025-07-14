# Top Jaw Documentation

## Operation Overview
- **Operation Name:** Face1
- **Toolpath Type:** Linearized circular move - low memory mode enabled

## Operation 1 Details

### Tool 1: 3 Flute DLC
- **Tool Number:** T9
- **Tool Size:** 6mm
- **RPM:** 15,000
- **Feed Rate:** 333.3 mm/min (for Z movement)
- **Operation Type:** Face Milling with Adaptive Pass
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)
- **Adaptive Pass:** Involves multiple passes with complex contour following, allowing for efficient material removal while maintaining consistent engagement with the workpiece.

### Tool 2: 4.2mm Drill
- **Tool Number:** T11
- **Tool Size:** 4.2mm
- **RPM:** 12,000
- **Feed Rate:** Not specified in the provided G-code.
- **Operation Type:** Drilling
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)

### Tool 3: Double Flute 3mm Ball
- **Tool Number:** T2
- **Tool Size:** 3mm
- **RPM:** 10,000
- **Feed Rate:** Not specified in the provided G-code.
- **Operation Type:** Scallop
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)

### Tool 4: Chamfer Mill
- **Tool Number:** T6
- **Tool Size:** 6mm
- **RPM:** 20,000
- **Feed Rate:** 333.3 mm/min
- **Operation Type:** 2D Chamfer
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)

### Tool 5: M5x0.8mm Thread Mill
- **Tool Number:** T17
- **Tool Size:** M5x0.8mm
- **RPM:** 6,000
- **Feed Rate:** Not specified in the provided G-code.
- **Operation Type:** Thread Milling
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)

## Operation 2 Details

### Tool 1: 3 Flute DLC
- **Tool Number:** T9
- **Tool Size:** 6mm
- **RPM:** 15,000
- **Feed Rate:** 333.3 mm/min (for Z movement)
- **Operation Type:** Face Milling with Adaptive Pass
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)
- **Adaptive Pass:** Involves multiple passes with complex contour following, allowing for efficient material removal while maintaining consistent engagement with the workpiece.

### Tool 2: Chamfer Mill
- **Tool Number:** T6
- **Tool Size:** 6mm
- **RPM:** 20,000
- **Feed Rate:** 333.3 mm/min
- **Operation Type:** 2D Chamfer
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)

## Summary of Operations
1. **Initial Setup and Probing:**
   - Probes reference surface.
   - Uses WCS 1 (G54).
   - Probes origin in current WCS.
   - Enables rotation compensation.

2. **Main Operation (Tool 1 - T9):**
   - **Type:** Face Milling with Adaptive Pass
   - **RPM:** 15,000
   - **Feed Rate:** 333.3 mm/min
   - **Operation:** Multiple passes with complex contour following, including adaptive milling strategies.

3. **Secondary Operations (Tool 2 - T11):**
   - **Type:** Drilling
   - **RPM:** 12,000
   - **Feed Rate:** Not specified.
   - **Operation:** Drilling operations as needed.

4. **Additional Operations (Tool 3 - T2):**
   - **Type:** Scallop
   - **RPM:** 10,000
   - **Feed Rate:** Not specified.
   - **Operation:** Scalloping as part of the machining process.

5. **Chamfer Operation (Tool 4 - T6):**
   - **Type:** 2D Chamfer
   - **RPM:** 20,000
   - **Feed Rate:** 333.3 mm/min
   - **Operation:** Chamfering around the perimeter.

6. **Threading Operation (Tool 5 - T17):**
   - **Type:** Thread Milling
   - **RPM:** 6,000
   - **Feed Rate:** Not specified.
   - **Operation:** Thread milling as required.

## Additional Notes
- The operation includes extensive safety checks and spindle controls.
- The G-code is designed for a specific firmware configuration (RRF) and includes automatic probing and work coordinate system management.
- The operation features multiple tool changes and complex machining paths.


# Machining Details for Large Sliding Base - Op1

### Steps:
1. **Initial Setup:**
   - Probes reference surface.
   - Switch to WCS 1 (G54).
   - Probes origin in current WCS.
   - Enables rotation compensation.

2. **Starting Position:**
   - Move to starting position in X and Y: `G0 X54.01 Y-2.395`
   - Move to starting position in Z: `G0 Z15.0`

3. **Engage Tool:**
   - Move down to Z position: `G1 Z-2.1 F333.3`

4. **Face Milling Operation:**
   - Perform linearized circular moves to mill the face:
     - `G1 X54.003 Z-2.194 F2000.0`
     - Continue with a series of linear moves to create the desired contour.

5. **Adaptive Pass:**
   - Execute adaptive milling strategies with multiple passes to efficiently remove material while maintaining consistent engagement with the workpiece.

6. **Final Positioning:**
   - Return to Z position: `G0 Z5.0`
   - Move to a new X and Y position: `G0 X10.896 Y138.867`
   - Engage tool again: `G1 Z-7.175 F333.3`
   - Perform additional milling operations as needed.

### Tool 1: 3 Flute DLC
- **Tool Number:** T9
- **Tool Size:** 6mm
- **RPM:** 15,000
- **Feed Rate:** 333.3 mm/min (for Z movement)
- **Operation Type:** Face Milling with Adaptive Pass
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)

### Tool 2: Single Flute 3mm
- **Tool Number:** T1
- **Tool Size:** 3mm
- **RPM:** Not specified in the G-code.
- **Feed Rate:** Not specified in the G-code.
- **Operation Type:** Not explicitly defined in the provided G-code.
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)

#### Steps:
1. **Engage Tool:**
   - Tool is passed to firmware but not explicitly used in the provided G-code.

### Tool 3: Chamfer Mill
- **Tool Number:** T6
- **Tool Size:** 6mm
- **RPM:** Not specified in the G-code.
- **Feed Rate:** Not specified in the G-code.
- **Operation Type:** Chamfering
- **Coolant:** Mist (M7)
- **Variable Spindle Speed Control:** Enabled (P4000 V200)

#### Steps:
1. **Engage Tool:**
   - Tool is passed to firmware but not explicitly used in the provided G-code.

## Summary of Operations
1. **Initial Setup and Probing:**
   - Probes reference surface.
   - Uses WCS 1 (G54).
   - Probes origin in current WCS.
   - Enables rotation compensation.

2. **Main Operation (Tool 1 - T9):**
   - **Type:** Face Milling with Adaptive Pass
   - **RPM:** 15,000
   - **Feed Rate:** 333.3 mm/min
   - **Operation:** Multiple passes with complex contour following, including adaptive milling strategies.

3. **Additional Operations:**
   - **Tool 2 (Single Flute 12mm):** Not explicitly used in the operation.
   - **Tool 3 (Chamfer Mill):** Not explicitly used in the operation.

## Additional Notes
- The operation includes extensive safety checks and spindle controls.
- The G-code is designed for a specific firmware configuration (RRF) and includes automatic probing and work coordinate system management.
- The operation features multiple tool changes and complex machining paths.