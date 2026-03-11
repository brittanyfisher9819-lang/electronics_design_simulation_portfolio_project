# Electronics Design and Simulation Portfolio Project

A GitHub-ready portfolio project for an **Electronics Design and Simulation Specialist**.  
This repository presents a compact but credible workflow covering:

- schematic design planning
- PCB layout deliverables
- SPICE-based circuit simulation
- documentation of methods and results

## Project Overview

The sample project is a **regulated sensor interface board** built around three practical blocks:

1. **Power stage** — 12 V input regulated to 5 V with filtering
2. **Signal conditioning** — op-amp based amplification and filtering for a sensor input
3. **Output stage** — comparator threshold detection driving an LED indicator

The repo includes:
- KiCad-style project notes and a netlist-like connection file
- LibrePCB placeholder project structure
- Ngspice simulation decks
- Qucs-S compatible netlists and notes
- generated plots and result summaries
- a polished case-study write-up

## Repository Structure

```text
eda_portfolio_project/
├── assets/
├── docs/
├── hardware/
│   ├── kicad/
│   └── librepcb/
├── results/
└── simulation/
    ├── ngspice/
    └── qucs-s/
```

## Tools Represented

| Tool | Use in this repo |
|---|---|
| KiCad | PCB/schematic project structure and design notes |
| LibrePCB | Alternative layout workflow placeholder and documentation |
| Ngspice | Transient and AC simulation decks |
| Qucs-S | Cross-tool simulation notes and example netlist |

## Main Design Goal

The design accepts a noisy low-level sensor signal, filters and amplifies it, then compares it against a threshold to produce a clear digital-style indicator.

## Key Files

| File | Purpose |
|---|---|
| `hardware/kicad/sensor_interface_connections.md` | Schematic-style signal and power connectivity |
| `simulation/ngspice/sensor_frontend_transient.cir` | Time-domain simulation deck |
| `simulation/ngspice/filter_ac_response.cir` | AC sweep deck |
| `simulation/qucs-s/comparator_threshold_demo.sch.txt` | Qucs-S style textual schematic description |
| `docs/case_study.md` | Portfolio-friendly explanation of the project |
| `results/simulation_summary.md` | Summary of design outcomes |

## Typical Results

- regulated 5 V rail from 12 V input
- filtered and amplified sensor waveform
- comparator switching when signal crosses threshold
- frequency response showing low-pass behavior

## How to Use This Repository

### 1. Upload to GitHub
Upload the contents of this repository to a new GitHub repo.

### 2. Add visuals
For a stronger portfolio, add:
- real schematic screenshots
- PCB layout screenshots
- simulation waveform exports
- rendered board images if available

### 3. Mention it in applications
A clean description:
> Electronics design and simulation portfolio project featuring schematic planning, PCB design documentation, and SPICE-based analysis using KiCad, Ngspice, and Qucs-S.

## Notes

This is a **portfolio demonstration project** designed to showcase workflow, documentation quality, and technical thinking.  
It avoids fabricated claims of manufactured hardware while still presenting realistic engineering artifacts.

## License

MIT
