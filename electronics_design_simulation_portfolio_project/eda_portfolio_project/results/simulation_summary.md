# Simulation Summary

## Results Overview

### Transient behavior
The transient deck models a sinusoidal sensor input, filters it, amplifies it, and compares it to a fixed threshold.

### AC behavior
The RC stage shows expected low-pass behavior with attenuation increasing as frequency rises.

## Interpreted Outcomes

| Observation | Meaning |
|---|---|
| Filter smooths the raw input | Noise is reduced before amplification |
| Amplifier increases signal swing | Weak sensor output becomes easier to evaluate |
| Comparator switches near threshold | Output becomes easy to use for downstream logic |
| AC response rolls off at high frequency | Front end favors low-frequency sensor content |

## Portfolio Value

This project demonstrates:
- circuit decomposition
- simulation readiness
- documentation clarity
- open-source EDA workflow familiarity
