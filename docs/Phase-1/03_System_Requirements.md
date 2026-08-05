\# System Requirements Specification (SRS)



\## 1. Introduction



The System Requirements Specification (SRS) defines the functional and non-functional requirements for the proposed \*\*32-bit Low-Power RISC-V Processor Core\*\*. This document serves as the foundation for the processor design and provides clear guidelines for architecture development, RTL implementation, verification, and physical design.



The processor will be designed using \*\*Verilog HDL\*\* based on the \*\*RV32I instruction set architecture\*\* and will follow the complete \*\*RTL-to-GDSII design flow\*\*.



\---



\# 2. Functional Requirements



The processor shall support the following functions:



\### 2.1 Instruction Fetch



\- Fetch instructions sequentially from instruction memory.

\- Update the Program Counter (PC) correctly after each instruction.

\- Support branch and jump instructions.



\### 2.2 Instruction Decode



\- Decode all supported RV32I instructions.

\- Generate the required control signals.

\- Extract opcode, register addresses, function fields, and immediate values.



\### 2.3 Arithmetic and Logic Operations



The processor shall execute:



\- ADD

\- SUB

\- ADDI

\- AND

\- OR

\- XOR

\- SLL

\- SRL

\- SRA

\- SLT

\- SLTU



\### 2.4 Memory Operations



The processor shall support:



\- Load Word (LW)

\- Store Word (SW)



\### 2.5 Branch Operations



The processor shall support:



\- BEQ

\- BNE



\### 2.6 Jump Operations



The processor shall support:



\- JAL



\### 2.7 Register File



The processor shall:



\- Contain 32 general-purpose registers.

\- Support two read ports.

\- Support one write port.

\- Keep register x0 permanently connected to zero.



\---



\# 3. Non-Functional Requirements



The processor shall satisfy the following non-functional requirements.



\## 3.1 Performance



\- Efficient execution of supported instructions.

\- Low instruction latency.

\- Stable operation under continuous execution.



\## 3.2 Power



\- Minimize dynamic power consumption.

\- Reduce unnecessary switching activity.

\- Support future low-power optimization techniques.



\## 3.3 Reliability



\- Correct execution of all supported instructions.

\- Stable behavior during reset and normal operation.

\- Reliable memory access.



\## 3.4 Scalability



The design shall allow future enhancements, including:



\- Pipelined architecture

\- Cache memory

\- Interrupt handling

\- Additional RISC-V instruction extensions



\---



\# 4. Hardware Requirements



The following hardware resources are required for development and verification.



| Component | Requirement |

|-----------|-------------|

| Processor Architecture | RISC-V RV32I |

| Word Length | 32-bit |

| Register Count | 32 |

| HDL | Verilog HDL |

| Clock | Single Clock |

| Development PC | Windows/Linux System |

| RAM | Minimum 8 GB (16 GB Recommended) |

| Storage | Minimum 20 GB Free Space |



\---



\# 5. Software Requirements



The project will use the following software tools.



| Tool | Purpose |

|------|---------|

| VS Code | RTL Development |

| Git | Version Control |

| GitHub | Repository Management |

| Icarus Verilog | Simulation |

| GTKWave | Waveform Analysis |

| Yosys | Logic Synthesis |

| OpenSTA | Static Timing Analysis |

| OpenROAD | RTL-to-GDSII Flow |

| Magic VLSI | Layout Visualization |

| Netgen | LVS Verification |



\---



\# 6. Design Constraints



The processor design shall satisfy the following constraints.



\- Based on the RV32I instruction set.

\- 32-bit architecture.

\- Modular RTL design.

\- Verilog HDL implementation.

\- Single-cycle architecture in the initial phase.

\- Compatible with open-source EDA tools.

\- Designed for future pipeline implementation.



\---



\# 7. Assumptions



The following assumptions are considered during the design.



\- Instruction memory is preloaded before execution.

\- Data memory is available during simulation.

\- The processor operates with a single clock source.

\- Reset initializes the processor correctly.

\- Only RV32I instructions are supported in the initial implementation.



\---



\# 8. Success Criteria



The project will be considered successful if it achieves the following:



\- Correct execution of all supported RV32I instructions.

\- Successful RTL simulation and functional verification.

\- Passing all designed testbenches.

\- Successful logic synthesis.

\- Successful timing analysis.

\- Power analysis completed.

\- Physical design completed using RTL-to-GDSII flow.

\- Generation of the final GDSII layout.



\---



\# 9. Summary



This System Requirements Specification establishes the technical requirements for the proposed Low-Power RISC-V Processor Core. These requirements will guide every stage of the project, including processor architecture, RTL coding, verification, synthesis, timing analysis, power optimization, and physical implementation.



The next phase of the project focuses on designing the processor architecture and defining the internal datapath, control unit, memory organization, and instruction formats before beginning RTL development.

