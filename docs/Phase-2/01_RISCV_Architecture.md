\# RISC-V Processor Architecture



\## 1. Introduction



The processor architecture defines the overall organization and interaction of all hardware components within the proposed Low-Power RISC-V Processor Core.



This project implements a \*\*32-bit RISC-V processor\*\* based on the \*\*RV32I instruction set architecture\*\* using a \*\*single-cycle datapath\*\*. The architecture is designed to be modular, making it easier to develop, verify, optimize, and extend in future versions.



The processor is intended for educational, research, and embedded system applications while demonstrating the complete RTL-to-GDSII design methodology.



\---



\# 2. Why RISC-V?



RISC-V is an open-standard Instruction Set Architecture (ISA) that provides flexibility, simplicity, and scalability without licensing restrictions.



The key advantages include:



\- Open-source architecture

\- Modular ISA

\- Simple instruction format

\- Easy hardware implementation

\- Suitable for embedded systems

\- Large academic and industrial adoption



These characteristics make RISC-V an ideal choice for designing a custom low-power processor.



\---



\# 3. Processor Overview



The proposed processor consists of several interconnected hardware modules.



The major components include:



\- Program Counter (PC)

\- Instruction Memory

\- Control Unit

\- Register File

\- Immediate Generator

\- Arithmetic Logic Unit (ALU)

\- Data Memory

\- Branch and Jump Logic

\- Multiplexers

\- Top-Level Processor Module



Each module performs a dedicated function while interacting with other modules to execute RV32I instructions.



\---



\# 4. Processor Characteristics



| Parameter | Value |

|-----------|-------|

| ISA | RV32I |

| Word Size | 32-bit |

| Processor Type | RISC |

| Execution Model | Single-Cycle |

| Register Count | 32 |

| Register Width | 32-bit |

| Memory Type | Harvard Architecture |

| HDL | Verilog HDL |



\---



\# 5. Architectural Design Decisions



The following design decisions are adopted for this project.



\- Single-cycle execution for simplicity.

\- Separate instruction and data memories.

\- Hardwired control unit.

\- Modular RTL implementation.

\- Open-source EDA tool flow.

\- Future support for pipelining and clock gating.



\---



\# 6. Processor Modules



The processor architecture includes the following functional modules.



\## Program Counter



Maintains the address of the next instruction.



\## Instruction Memory



Stores program instructions.



\## Register File



Stores 32 general-purpose registers.



\## Immediate Generator



Generates immediate values from instructions.



\## Control Unit



Generates processor control signals.



\## ALU



Performs arithmetic and logical operations.



\## Data Memory



Stores program data.



\## Branch Unit



Handles conditional branch decisions.



\---



\# 7. Execution Flow



The processor executes each instruction using the following sequence.



1\. Fetch instruction.

2\. Decode instruction.

3\. Read registers.

4\. Generate immediate value.

5\. Execute ALU operation.

6\. Access memory if required.

7\. Write result back.

8\. Update Program Counter.



\---



\# 8. Future Enhancements



The architecture is designed to support future improvements such as:



\- Five-stage pipelining

\- Forwarding unit

\- Hazard detection

\- Cache memory

\- Clock gating

\- Additional RISC-V instruction extensions



\---



\# 9. Summary



This document defines the overall architecture of the proposed Low-Power RV32I Processor. It establishes the processor organization and the interaction between its hardware modules, providing the foundation for the datapath design and RTL implementation.

