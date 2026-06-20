# MIPS-Processor

This repository contains hardware designs and implementations for custom MIPS architectures and FPGA accelerators.

---

## Mini MIPS Processor (32-bit Multi-Cycle)
**Academic Project** | *CS220 - Prof. Mainak Chaudhuri *

A custom-designed 3-cycle, 32-bit MIPS processor implemented in Verilog. It is built to support a robust Instruction Set Architecture (ISA) including complex arithmetic, control flow, and memory operations.

### Key Architecture & Features
* **Custom Datapath:** Engineered a custom ALU and Register File to comprehensively support complex arithmetic, branch/jump control flow operations, and aligned big-endian load/store instructions.
* **FSM Control Path:** Optimized the control logic utilizing a 3-state Finite State Machine (FSM) architecture. This resolved critical data path timing failures and successfully met a strict **10ns clock constraint**.
* **I/O Synchronization:** Designed hardware stalling mechanisms to flawlessly synchronize dynamic keyboard inputs and unbounded I/O streams.
* **System-on-Chip Integration:** Packaged and integrated the processor as a custom **AXI4 IP** using Xilinx Vivado.
* **Validation:** Verified functional hardware correctness by executing MIPS assembly code directly through the Vitis IDE.

