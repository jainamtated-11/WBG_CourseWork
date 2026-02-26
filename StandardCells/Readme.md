
# Standard Cells — WBG Course Project

This repository contains transistor-level implementations and simulations of basic CMOS standard logic gates designed as part of the WBG Course Project. The designs include Inverter (INV), 2-input NAND, and 2-input NOR logic cells with transistor-level simulation using NGSpice, physical layout using Magic VLSI, and digital verification using IRSIM.

## Overview

This project demonstrates the complete VLSI design flow for basic standard cells:
- Transistor-level schematic design
- SPICE simulation and waveform verification
- Physical layout implementation
- Digital functional verification

## Logic Cells Implemented

- INV — CMOS Inverter
- NAND2 — 2-input NAND gate
- NOR2 — 2-input NOR gate

Each cell includes:
- MOS transistor implementation (PMOS + NMOS network)
- NGSpice netlist and testbench
- Magic layout file (.mag)
- IRSIM simulation setup and stimulus vectors

## NGSpice Simulation

NGSpice is used for transistor-level analog simulation to verify voltage transfer characteristics and transient response.

To run simulation:
cd ngspice
ngspice <cell_name>.cir

Simulations verify:
- Correct logic functionality
- Output waveform behavior
- Switching characteristics

## Magic Layout

Layouts are designed using Magic VLSI layout tool following standard CMOS layout rules.

To open layout:
magic <cell_name>.mag

Layouts ensure:
- Proper transistor placement
- Correct routing of metal layers
- DRC-clean design

## IRSIM Verification

IRSIM is used for digital-level simulation to confirm logical correctness using input vectors.

To run:
irsim <cell_name>.vec > output.txt

This verifies correct truth-table behavior of each gate.

## Tools Used

- NGSpice — Circuit simulation
- Magic — Layout design
- IRSIM — Digital logic simulation

## Objective

The objective of this project is to understand the complete standard cell design flow from schematic to layout and functional verification.

## Author

Gunja Jaswanth
