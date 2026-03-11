# Case Study

## Context

This portfolio project demonstrates a small but realistic mixed-signal electronics workflow. The design objective is to convert a noisy analog sensor signal into a stable thresholded output using a regulated power stage, analog conditioning, and a comparator.

## Design Blocks

### Power Regulation
The board assumes a 12 V DC input and generates a clean 5 V rail for the analog stage. Decoupling capacitors and local bypassing are included in the design notes.

### Analog Front End
A weak sensor signal is passed through:
- an RC low-pass filter
- a non-inverting amplifier stage
- an offset / reference comparison stage

### Comparator Output
A comparator monitors the conditioned signal and drives an indicator LED when the threshold is crossed.

## Why This Project Works as a Portfolio Sample

It demonstrates:
- practical block decomposition
- mixed analog and digital reasoning
- SPICE simulation literacy
- engineering documentation habits
- compatibility with open-source EDA tools

## Deliverables

- schematic connectivity notes
- simulation decks
- project assumptions
- results interpretation
- implementation notes for future PCB layout refinement

## Future Enhancements

- add a real KiCad `.kicad_sch` and `.kicad_pcb`
- add BOM and manufacturing outputs
- include measured data from a prototype board
- expand simulation coverage with Monte Carlo or tolerance sweeps
