# 6-GHz-RF-Signal-Generator

This project is a high-frequency RF signal generator module designed to generate a fixed 6.3 GHz signal and deliver it through an SMA connector. The design uses a voltage-controlled oscillator, RF power amplifier, low-noise power regulation, dual-rail biasing, and controlled-impedance RF routing.

The project focuses on RF signal generation, high-frequency PCB layout, impedance control, AC coupling, biasing, power filtering, and SMA-based RF output design.

## Key Features

- Fixed 6.3 GHz RF output
- SMA connector output interface
- HMC358MS8GE voltage-controlled oscillator
- HMC637ALP5E RF power amplifier
- Approximately 13 dB amplifier gain
- Low-noise regulator for main supply
- Dual-rail regulator for amplifier gate voltages
- Optional VTUNE header for frequency adjustment
- AC-coupled RF input and output paths
- Bias-tee network for RF/DC isolation
- 50 ohm controlled-impedance RF routing
- Four-layer PCB stack-up with RF-aware layout

## Major Components

| Component | Function | 
|---|---|
| HMC358MS8GE | Voltage-controlled oscillator generating the RF carrier |
| HMC637ALP5E | RF power amplifier providing signal gain |
| TPS562201 | Low-noise regulator for main supply voltage |
| LM27762DSSR | Dual-rail regulator for amplifier gate biasing |
| SMA Connector | RF output interface |
| Bias-Tee Network | Isolates DC supply from RF signal path |

## Design Approach

The HMC358MS8GE VCO generates the 6.3 GHz carrier signal. The signal is AC-coupled into the HMC637ALP5E RF amplifier, which boosts the signal before sending it to the SMA connector.

The power section includes a low-noise regulator for the main supply and a dual-rail regulator for the amplifier gate bias voltages. Proper filtering and decoupling are used to reduce supply noise that could affect the RF output.

The PCB layout uses controlled-impedance routing for RF traces, short signal paths, RF/DC separation, and a four-layer stack-up. Special attention is given to 50 ohm routing, coplanar waveguide layout, AC coupling, bias-tee design, and minimizing parasitic coupling between the RF and power sections.

## Project Files

- [Schematic Diagram](https://github.com/harinibabu63/-6-GHz-RF-Signal-Generator/blob/main/6GHZ%20RF%20signal%20generator.png)
- [NC Drill](https://github.com/harinibabu63/-6-GHz-RF-Signal-Generator/blob/main/NC%20drill%206GHZ%20RF%20signal%20Generator.png)
- [Bill of Materials](https://github.com/harinibabu63/-6-GHz-RF-Signal-Generator/blob/main/BOM_6GHZ%20generator.png)

## What I Learned

- RF signal generation using a VCO
- High-frequency PCB layout practices
- 50 ohm controlled-impedance routing
- RF amplifier biasing 
- AC coupling in RF signal paths
- Bias-tee circuit design
- Low-noise power supply design
- Decoupling and filtering for RF circuits
- SMA connector integration
- Four-layer RF PCB layout strategy
