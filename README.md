SHA3-256 Implementation

Overview

This project implements the SHA3-256 cryptographic hash function in Verilog. SHA3-256 is a part of the SHA-3 family, based on the Keccak algorithm, and produces a 256-bit hash output from an arbitrary-length input. This implementation is designed for FPGA acceleration and integration with RISC-V architectures.

Features

Implements the SHA3-256 hashing algorithm based on the Keccak sponge construction.

Supports arbitrary-length message inputs.

Optimized for hardware efficiency with pipelined processing.

Compatible with FPGA-based cryptographic accelerators.

Designed for integration with the Wishbone protocol for RISC-V systems.

Project Structure

SHA3-256/
│-- src/                   # Verilog source files
│   │-- sha3_256.sv        # Top-level SHA3-256 module
│   │-- chi.sv             # Keccak Chi transformation
│   │-- fn_top.sv          # Keccak function top module
│   │-- iota.sv            # Keccak Iota transformation
│   │-- padding.sv         # SHA3 message padding logic
│   │-- pi.sv              # Keccak Pi transformation
│   │-- rho.sv             # Keccak Rho transformation
│   │-- theta.sv           # Keccak Theta transformation
│   │-- top.sv             # Integration and control module
│-- testbench/             # Testbenches for verification
│   │-- sha3_tb.v          # Testbench for SHA3-256 verification
│-- firmware/              # Integration firmware for RISC-V
│-- docs/                  # Documentation and design notes
│-- README.md              # Project documentation

Installation & Usage

Prerequisites

Verilog/SystemVerilog simulator (e.g., ModelSim, Verilator, Icarus Verilog)

FPGA toolchain (e.g., Yosys, Quartus, Vivado for synthesis)

RISC-V toolchain (if integrating with RISC-V processors)
