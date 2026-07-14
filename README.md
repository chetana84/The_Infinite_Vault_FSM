# The Infinite Vault – Multi-Phase FSM Security System

## Overview

The Infinite Vault is a modular multi-phase Finite State Machine (FSM) security system designed and implemented in **Verilog HDL** using **Xilinx Vivado**. The project simulates a digital vault escape challenge consisting of five sequential security phases. A centralized top-level FSM coordinates each phase, ensuring successful completion before advancing to the next stage while handling failures through checkpoint-based recovery.

This project demonstrates RTL design principles, hierarchical FSM implementation, modular hardware architecture, and functional verification through simulation.

---

## Features

- Hierarchical top-level FSM controller
- Five independent Verilog modules for each security phase
- Sequential phase execution with state-based control
- Serial and parallel input validation
- Timed output sequence generation
- Automatic failure detection and checkpoint recovery
- Modular and reusable RTL architecture
- Behavioral simulation and functional verification in Vivado

---

## Security Phases

### Phase 1 – Code Lock
- Verifies a 4-bit serial input sequence (`1011`).

### Phase 2 – Switch Room
- Validates a 4-bit parallel switch combination (`1101`).

### Phase 3 – Maze Tracker
- Checks a predefined sequence of directional inputs using an FSM.

### Phase 4 – Pressure Plates
- Verifies three consecutive 8-bit pressure plate patterns.

### Phase 5 – Time Lock
- Generates a timed three-step output sequence to complete the vault unlocking process.

---

## Tools & Technologies

- Verilog HDL
- Xilinx Vivado
- RTL Design
- Finite State Machines (FSM)
- Behavioral Simulation

---

## Project Structure

```
The-Infinite-Vault-FSM/
│
├── rtl/
│   ├── top_module.v
│   ├── phase1.v
│   ├── phase2.v
│   ├── phase3.v
│   ├── phase4.v
│   └── phase5.v
│
├── testbench/
│   └── top_tb.v
│
├── images/
│   ├── block_diagram.png
│   ├── fsm_diagram.png
│   └── simulation_waveforms.png
│
├── docs/
│   └── Project_Report.pdf
│
└── README.md
```

---

## Learning Outcomes

- Finite State Machine (FSM) Design
- Sequential Logic Design
- Modular RTL Development
- Digital Hardware Verification
- Hierarchical Hardware Design
- Functional Simulation using Vivado

---

## Author

**Chetana**

