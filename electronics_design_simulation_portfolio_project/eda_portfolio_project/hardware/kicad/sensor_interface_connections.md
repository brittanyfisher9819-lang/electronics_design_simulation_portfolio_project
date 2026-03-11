# Sensor Interface Connections

## Main Nets

| Net | Description |
|---|---|
| VIN_12V | Main 12 V input rail |
| GND | Common ground |
| VREG_5V | Regulated 5 V rail |
| SENSOR_IN | Raw analog sensor input |
| FILTERED_IN | Filtered sensor node |
| AMP_OUT | Amplified analog output |
| VREF_2V5 | Comparator reference |
| COMP_OUT | Comparator digital output |
| LED_DRIVE | Indicator LED net |

## Functional Connectivity

1. `VIN_12V` feeds the regulator input.
2. Regulator output creates `VREG_5V`.
3. `SENSOR_IN` passes through an RC filter to `FILTERED_IN`.
4. `FILTERED_IN` enters the non-inverting amplifier stage.
5. Amplifier output appears at `AMP_OUT`.
6. Comparator compares `AMP_OUT` to `VREF_2V5`.
7. Comparator output drives LED current-limited indicator through `LED_DRIVE`.

## Suggested Components

| Reference | Suggested Part Type | Role |
|---|---|---|
| U1 | 5 V linear regulator | Power regulation |
| U2 | Rail-to-rail op-amp | Signal amplification |
| U3 | Comparator | Threshold detection |
| R1, C1 | RC filter pair | Noise suppression |
| R2, R3 | Gain-setting resistors | Amplifier configuration |
| R4, R5 | Divider resistors | Reference generation |
| D1 | LED | Output indicator |
| R6 | Resistor | LED current limiting |
