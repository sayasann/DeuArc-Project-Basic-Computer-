# DEUARC: DEU Electronic Universal Automatic Reduced Computer


![DEUARC](https://github.com/user-attachments/assets/ec363474-f1eb-4c0a-95b8-ad35ba4435a7)



This project was developed as part of the CME2206 Computer Architecture course at Dokuz Eylul University. DEUARC (DEU Electronic Universal Automatic Reduced Computer) is designed to demonstrate the fundamental components and operational logic of a basic computer architecture.

# 📌 Project Purpose

DEUARC is built with 9 registers, 3 memory units (instruction, data, and stack), an arithmetic and logic unit (ALU), a control unit (CU), and a common bus system. The goal is to provide hands-on experience on how these components work and communicate with each other.

# 🏗️ General Structure

    Registers:

        Address Register (AR)

        Program Counter (PC)

        Stack Pointer (SP)

        Input Register (INPR)

        Output Register (OUTR)

        Instruction Register (IR)

        3 General Purpose Registers (R0, R1, R2)

    Memory:

        Instruction Memory (32x11)

        Data Memory (16x4)

        Stack Memory (16x5)

    Common Bus System:
    Enables data exchange between different components.

    ALU (Arithmetic and Logic Unit):
    Executes basic arithmetic and logic operations.

    Control Unit:
    Decodes instructions and generates control signals to coordinate the execution of micro-operations in registers, memories, and the ALU.

# 🔧 Tools Used

    Quartus II:
    Used for simulation and design verification of the project.

# 📜 Instruction Set

The instruction set is defined by a 4-bit opcode and a 1-bit Q bit, supporting 16 instructions.
Here are some of the core instructions:
Instruction	Opcode	Description
HLT	0111	Halts the computer
ADD	0000	Adds S1 and S2, stores result in Rd
INC	0001	Increments S1, stores result in Rd
AND	0010	ANDs S1 and S2, stores result in Rd
NOT	0011	Complements S1, stores result in Rd
DBL	0101	Doubles S1, stores result in Rd
DBT	0110	Divides S1 by 2, stores result in Rd
ST	1000	Writes Rd content or S1S2 into memory
LD	1001	Loads memory content into Rd
IO	1010	Handles input/output data transfers
JMP	1100	Jumps to address (conditional or unconditional)
CAL	1101	Calls address and pushes PC onto the stack (PUSH)
RET	1110	Returns PC from stack (POP)
JMR	1111	Relative jump to an address offset

Each instruction triggers specific micro-operations based on its opcode and the Q bit.

# 🧩 Control Unit (CU)

    Decodes instruction opcodes

    Generates timing signals (T0, T1, T2, …)

    Sends control signals to ALU, registers, and memories

    Ensures proper sequencing of micro-operations


# 💡 Usage

1️⃣ Open the simulation files in Quartus II.
2️⃣ Run simulations and capture waveform outputs for verification.
3️⃣ Submit all simulation files for each lab session.

# ⚠️ License and Usage

This project is shared for educational and personal portfolio purposes only.
Copying, distribution, or use of this project without explicit permission is strictly prohibited.

# ✏️ Written by


Example:

    Author: Serkan Ayaşan & Orhan Rzayev

    

    
