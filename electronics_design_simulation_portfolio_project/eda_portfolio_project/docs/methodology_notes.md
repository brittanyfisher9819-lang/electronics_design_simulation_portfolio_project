# Methodology Notes

## Assumptions

- Input supply: 12 V DC
- Regulated rail: 5 V
- Sensor input amplitude: approximately 50 mV to 300 mV before amplification
- Target comparator threshold: 2.5 V
- Amplifier gain target: about 10x to 15x depending on component choice

## Workflow

1. Define functional blocks and interfaces
2. Draft connectivity and component intent
3. Simulate transient response in Ngspice
4. Simulate frequency response for the input filter
5. Mirror the design logic in Qucs-S style documentation
6. Package design as a portfolio artifact

## Engineering Focus

The emphasis is not just the final circuit, but the quality of the documentation and the ability to show reasoning clearly.
