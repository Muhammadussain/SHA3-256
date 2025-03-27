<h1>SHA3-256 FPGA Implementation</h1>
#Overview

This project implements the SHA3-256 cryptographic hash function in Verilog/SystemVerilog. SHA3-256 is part of the SHA-3 family, based on the Keccak algorithm, and produces a 256-bit hash output from an arbitrary-length input. The implementation is optimized for FPGA acceleration and designed for integration with RISC-V architectures using the Wishbone protocol.

Features

✅ Implements the SHA3-256 hashing algorithm based on the Keccak sponge construction
✅ Supports arbitrary-length message inputs
✅ Optimized for hardware efficiency with pipelined processing
✅ Compatible with FPGA-based cryptographic accelerators
✅ Designed for integration with RISC-V systems using the Wishbone protocol

Project Structure

📂 SHA3-256/ (Root Directory)├── 📁 src/ (Verilog source files)│  
├── sha3_256.sv → Top-level SHA3-256 module│   
├── chi.sv → Keccak Chi transformation│   
├── fn_top.sv → Keccak function top module│ 
├── iota.sv → Keccak Iota transformation│  
├── padding.sv → SHA3 message padding logic│ 
├── pi.sv → Keccak Pi transformation│  
├── rho.sv → Keccak Rho transformation│  
├── theta.sv → Keccak Theta transformation│ 
├── top.sv → Integration and control module
├── 📁 testbench/ (Testbenches for verification)│ 
├── toptb.sv → 
📄 README.md → Project documentation (this file)

Installation & Usage

Prerequisites

Ensure you have the following tools installed:

Verilog/SystemVerilog Simulator: ModelSim, Verilator, Icarus Verilog

FPGA Toolchain: Yosys, Quartus, Vivado (for synthesis)

RISC-V Toolchain: If integrating with a RISC-V processor
