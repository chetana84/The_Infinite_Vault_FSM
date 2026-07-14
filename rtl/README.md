# RTL Source Files

This directory contains the Register Transfer Level (RTL) implementation of **The Infinite Vault – Multi-Phase FSM Security System**. The design is written in **Verilog HDL** and developed.

## Module Description

| File | Description |
|------|-------------|
| `top_module.v` | Top-level FSM controller that manages the execution flow between all five security phases. It monitors the completion status of each phase and controls state transitions. |
| `phase1.v` | Implements the **Code Lock** module, which validates the 4-bit serial input sequence (`1011`). |
| `phase2.v` | Implements the **Switch Room** module, verifying the 4-bit parallel switch combination (`1101`). |
| `phase3.v` | Implements the **Maze Tracker** module, validating the predefined sequence of directional inputs using a finite state machine. |
| `phase4.v` | Implements the **Pressure Plates** module, which checks three sequential 8-bit input patterns for correctness. |
| `phase5.v` | Implements the **Time Lock** module, generating the required timed output sequence to complete the vault unlocking process. |

## Design Highlights

- Modular Verilog HDL implementation
- Hierarchical FSM architecture
- Sequential phase execution
- Independent phase modules
- Status-based phase transitions
- Failure detection and recovery logic
- Behavioral simulation using Xilinx Vivado

> **Note:** Each module is designed independently and integrated through the top-level controller, promoting modularity, readability, and easier verification.
