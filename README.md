# Custom 170W Synchronous Boost Converter PCB

A high-power synchronous boost converter designed for the MARS Rover onboard computing system, converting 12V input to 21V output at approximately 170W.

## Project Overview

This project covers the complete hardware development lifecycle of a high-power DC-DC boost converter, from circuit design and PCB layout through hardware bring-up, electrical measurements, and validation.

The converter was designed to provide a stable 21V supply for onboard computing systems while maintaining reliable high-current power delivery and minimizing noise coupling between power and feedback circuitry.

## Specifications

| Parameter | Value |
|---|---|
| Input Voltage | 12V |
| Output Voltage | 21V |
| Output Power | ~170W |
| Controller | LM5022 |
| PCB | 2-Layer |
| Design Tool | Altium Designer |
| Application | MARS Rover Onboard Computing |

## Converter Design

The converter was designed around the LM5022 controller and includes:

- MOSFET switching stage
- Current-sense network
- Feedback and compensation network
- Input filtering
- Output filtering
- Voltage-divider network
- High-current power routing

## PCB Design

The PCB was developed in Altium Designer, covering:

- Schematic capture
- Component selection and footprint assignment
- 2-layer PCB layout
- High-current power routing
- Copper pours
- Design Rule Checking (DRC)
- Current-density analysis

Current-density analysis was used to evaluate high-current traces and copper regions and optimize the power paths for reliable operation under continuous load.

## PCB Architecture

The PCB contains two electrically isolated copies of the boost-converter circuit, allowing the board to provide independent power outputs for two onboard Intel NUC computing systems.

## Hardware Validation

Following PCB design, the converter underwent hardware bring-up and electrical validation.

Validation included:

- Power-up testing
- Voltage measurements
- Output regulation checks
- Load testing
- Electrical debugging
- Measurement using Keysight test equipment
