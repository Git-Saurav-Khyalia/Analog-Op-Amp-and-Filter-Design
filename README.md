# Analog Circuit Design & Simulation | CMOS Op-Amp and Active Low-Pass Filter

**Tools:** LTspice · Python · Jupyter Notebook · Analog Circuit Design · CMOS Device Modeling

## Overview

This project explores two analog circuit design problems: a two-stage CMOS operational amplifier and a high-order active low-pass filter. The workflow combines analytical calculations, circuit implementation, simulation-based evaluation, and technical documentation.

The objective is to understand how circuit specifications translate into component values, transistor sizing, frequency-response requirements, and measurable performance characteristics.

The designs are intended for educational study and analog electronics interview preparation.

## Project Portfolio

### 1. Two-Stage CMOS Operational Amplifier

The operational amplifier design focuses on transistor-level sizing and performance evaluation against a set of target specifications.

**Design considerations**
- Small-signal gain and gain-bandwidth product (GBW)
- Slew rate and transient response
- Input common-mode range (ICMR)
- Output voltage swing
- Noise and device operating conditions
- MOSFET sizing and biasing considerations

**Design workflow**
1. Translate the target specifications into circuit-level requirements.
2. Perform analytical calculations to estimate transistor dimensions and operating conditions.
3. Implement the circuit and simulation test benches in LTspice.
4. Evaluate simulated behavior against the intended design targets.
5. Document the results, assumptions, and performance trade-offs.

**Key learning areas:** CMOS analog design, transistor sizing, biasing, small-signal analysis, and amplifier performance evaluation.

### 2. 11th-Order Butterworth Active Low-Pass Filter

The filter design investigates a high-order Butterworth response with a target passband edge of 14 kHz and a stopband target of 20 kHz.

**Design considerations**
- Butterworth magnitude response
- Filter-order selection and frequency-domain specifications
- Second-order Sallen–Key filter sections
- First-order gain stage
- Component-value calculations
- Frequency-response verification using LTspice

**Design workflow**
1. Translate the passband and stopband requirements into filter-design constraints.
2. Calculate the filter response and component values using the provided calculations notebook.
3. Implement the cascaded filter stages in LTspice.
4. Examine the simulated frequency response and compare it with the design targets.
5. Document the design approach, limitations, and relevant trade-offs.

**Key learning areas:** Active filter design, frequency response, transfer functions, filter-order selection, and analog simulation.

## Repository Structure

```text
.
├── op-amp-design/
│   ├── op_amp_calculations.ipynb
│   ├── LTspice schematics and symbols
│   └── op_amp_design_report.pdf
│
├── filter-design/
│   ├── filter_calculations.ipynb
│   ├── LPF.asc
│   ├── OPAMP.sub
│   └── filter_design_report.pdf
│
└── tests/
    └── validate_project.py
```

*The file listing above reflects the intended repository structure; adjust it to match the files actually present.*

## Tools and Technologies

| Tool | Purpose |
|---|---|
| LTspice | Analog circuit implementation and simulation |
| Python | Supporting calculations and numerical analysis |
| Jupyter Notebook | Documenting design calculations |
| SPICE models | Representing device and amplifier behavior in simulation |
| PDF reports | Recording design methodology and results |

## Validation

The repository includes a lightweight validation script intended to check notebook readability and the presence of expected design files.

Run it from the repository root:

```bash
python tests/validate_project.py
```

This is a repository-integrity check, not a substitute for electrical verification. Circuit validation requires running the simulations and evaluating their outputs against the design specifications.

## Engineering Scope and Limitations

- The work is simulation-based; hardware fabrication and bench measurements are not claimed.
- Simulated performance depends on the selected device models, component assumptions, operating conditions, and test-bench configuration.
- The supplied calculations and simulation results should be independently reviewed before any hardware implementation.
- The filter targets describe the intended design requirements; compliance should be confirmed from the actual frequency-response results.
- The validation script checks repository artifacts rather than proving circuit correctness.

## Skills Demonstrated

- Analog circuit analysis and design methodology
- CMOS transistor sizing and biasing concepts
- Operational amplifier performance specifications
- Active low-pass filter design
- Frequency-domain and transient simulation
- Analytical calculations and simulation-based verification
- Technical documentation and engineering trade-off analysis

## Intended Application

This project is relevant to the study of analog electronics, circuit simulation, semiconductor fundamentals, and entry-level analog design workflows. It provides a foundation for further exploration of transistor-level design, amplifier characterization, filter optimization, and hardware validation.
