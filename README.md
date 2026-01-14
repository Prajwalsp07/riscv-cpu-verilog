# riscv-cpu-verilog
This project is a complete single-cycle implementation of a RISC-V RV32I CPU core written from scratch in Verilog.
The objective of this project is to understand how a real instruction set architecture maps to hardware datapath and control logic at the RTL level.

The design prioritizes correctness and architectural clarity over performance optimizations such as pipelining.

# Instruction Support (RV32I)
Arithmetic and Logical (Register)
 -ADD, SUB
 -AND, OR, XOR
 -SLL, SRL, SRA

Arithmetic and Logical (Immediate)
 -ADDI
 -ANDI, ORI, XORI
 -SLTI, SLTIU

Memory Access
 -LW (Load Word)
 -SW (Store Word)

Control Flow
 -BEQ, BNE
 -BLT, BGE (signed)
 -BLTU, BGEU (unsigned)
 -JAL (Jump and Link)
 -JALR (Jump and Link Register)

Upper Immediate Instructions
 -LUI (Load Upper Immediate)
 -AUIPC (Add Upper Immediate to PC)

All listed instructions follow the RV32I specification and execute in a single clock cycle.
