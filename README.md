# 🛠️ MIPS Processor Simulator

[![Java Version](https://img.shields.io/badge/java-17%2B-orange.svg)](https://www.oracle.com/java/)
[![Architecture](https://img.shields.io/badge/architecture-MIPS--32-blue.svg)]()
[![Build](https://img.shields.io/badge/tests-passing-brightgreen.svg)]()

A comprehensive behavioral simulator for the MIPS-32 processor architecture implemented in Java. This tool parses, decodes, and simulates the execution of MIPS assembly instructions, managing registers, program counters, and memory states realistically.

---

### 🧠 System Architecture

The simulator replicates the standard MIPS execution cycle, breaking down instructions into their component fields (Opcode, RS, RT, RD, Shamt, Funct) to execute R-type, I-type, and J-type assembly operations.

* **Instruction Fetch & Decode:** Parses raw binary or hexadecimal assembly streams into structured software components.
* **Execution Engine:** Simulates ALU operations, branches, jumps, and data hazard evaluations.
* **Memory & Register File:** Maintains a robust 32-bit register file state along with data and instruction memory visualization.

### 📁 Repository Structure

```text
Processor-Simulator/
│
├── src/             # Core Java source code (Parsers, ALU, Registers, CPU logic)
├── tests/           # Unit tests and sample MIPS assembly validation scripts
├── docs/            # Technical specifications, ISA guides, and assignment reports
├── .gitignore
└── README.md

🚀 Getting Started
Prerequisites
  Java Development Kit (JDK) 17 or higher
  Any modern IDE like IntelliJ IDEA or Eclipse (Optional)

How to Run Tests
This repository includes a robust suite of unit tests to verify the correctness of individual instructions and pipeline state behaviors. Run them via your IDE or using the build tool command wrapper:
Shell
# Run unit tests to verify standard instruction set simulations
./gradlew test  # Or use Maven/IDE testing framework depending on project setup


🛠️ Supported Instructions
Type            Mnemonics
R-Type          add, sub, and, or, sll, srl, slt
I-Type          lw, sw, beq, bne, addi, andi, ori
J-Type          j, jal

---




