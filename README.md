# VSDSquadron Mini-INTERN

# Overview:
     1.TASK 1
     2.TASK 2
     3.TASK 3

# TASK 1

# DESCRIPTION:

A development board for RISC-V is the vsdsquadron mini. A 32-bit RISC-V core resides within it. It runs on a 24MHz frequency and contains 16KB of flash memory and 2KB of SRAM. Supporting protocols including SPI, USART, and I2C, the board contains fifteen GPIO pins.

# PROCESS:

The tasks at hand include installing Ubuntu on VMBox, Visual C++, and writing an example of C code along with analyzing RISC assembly code for the sample C code. These are the essential programs for this internship.

Installing Ubuntu on VMBox Open the Ubuntu terminal after installing the tools, then type the command.


Order for Installation of Leafpad apt-get install leafpad $ sudo

 $ cd $ leafpad filename.c & to launch Leafpad

 ![To Open Leafpad](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/5ac9fcc7-2363-4219-ad11-a9aa96f3ba2a)

 # PROGRAM:
 To Find the Sum Of Product

 ![TO FIND THE SUM PROGRAM](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/340df625-8b93-41f0-9fc6-7dbd6e40cea2)

 ![PROGRAM](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/094195cd-567e-46d8-9f0e-b532b6093524)

 # OUTPUT:
 The Output for the program is

 ![OUTPUT](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/24adcd66-17ca-454b-8960-3bb998bf0c58)

 Directing the compilation of RISC-V compiler code $rv64-unknown-elf-gcc-O1 -march=rv64i -mabi=lp64o filename.o filename.c $ -ltr filename.o

 ![To Open the Riscv Compiler](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/c233f032-012e-4414-992b-1fe71633c3f9)

 To view the assembly code, press. $ filename.o riscv64-unknown-elf-objdump-d ------>A lot of code is provided by $ riscv64-unknown-elf-objdump -d filename.o | less ------->offers Reduced Code/main and a way to view the main purpose of the code.

![ASSEMBLY CODE](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/c44881f9-3afd-4aae-a649-c256e9142ffc)

This facilitates navigation by opening the output in the less editor.
Using?main, we search for the keyword main.

![To Find Out Main](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/bba41f05-53f2-43be-be54-6e88f5021fec)

Guidelines for Analyzing Assembly Code RCV64-unknown-elf-gcc-Ofast -mabi=lp64 -march=rv64i -o filename.o filename.c Use $ riscv64-unknown-elf-objdump -d filename.o | less /main

![To command assembly program Ofast](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/17812fb0-9ae1-4a2c-80fb-dd522a90845f)

By utilizing a hexadecimal calculator and deducting the address numbers provided at the leftmost end, let's count the number of instructions that are executed in the main block.
The primary block of instructions consists of fifteen lines.
Let's use an alternative approach to the code compilation. -Ofast should be used in place of -O1.

![Output For Ofast Command](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/eab0fb76-989d-43b8-bb8a-ac86beea2342)

As we can see, there are now just 12 instructions, a decrease in the previous number of instructions.


# TASK 2

o Create a simple C code for the "Crafting a Digital Clock Divider Circuit" project, then use the RISC-V compiler to analyze assembly code instructions.

A circuit known as a clock cycle divider receives an input clock signal and outputs a clock signal with a frequency that is a fraction of the input frequency. This is frequently used to lower the clock signal frequency for different components in digital circuitry.

To create a simple clock cycle divider using a C program that can be compiled with RISC-V GCC, we will simulate the functionality of a digital clock divider circuit in software. This will involve a basic loop that simulates dividing a clock signal by counting cycles.

![leaf pad](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/ee863b93-0174-4ee2-acff-7b266513848d)

# PROGRAM:

Here is a simple C program that demonstrates this concept:

![clock divider program](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/9fa6ee1f-3635-4963-943e-063467305f87)

# EXPLANATION:

1. clock_divider function:

  Takes two parameters: divisor (the factor by which to divide the clock) and cycles (the number of clock cycles to simulate).
  Uses a counter to keep track of the number of cycles.
  Toggles the divided_clock signal whenever the counter reaches the divisor.

2. main function:

  Sets the divisor and cycles values.
  Calls the clock_divider function to perform the simulation.
  Prints out the state of the divided clock signal for each cycle.

# OUTPUT:

The Output for the program is

![clock divider output](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/13a3ae98-1e68-4b4a-903b-0d496485c281)

# Compilation with RISC-V GCC:

To compile this program with RISC-V GCC, follow these steps:

1.Install RISC-V GCC: Make sure you have the RISC-V GCC toolchain installed. You can download and install it from the official RISC-V website or use a package manager if available.

2.Save the Program: Save the above code to a file named clock_divider.c.

3.Compile the Program: Use the following command to compile the program With RISC-V GCC.

4.Run the Program: If you have a RISC-V emulator or hardware, you can run the compiled program. For example, using the QEMU emulator:

![risc v compiler](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/8ef3712c-b363-40f4-83e9-7a61a6c646b7)

Overseeing the RISC-V compiler code compilation $rv64-unknown-elf-gcc-O1 -mabi=lp64o filename.o filename.c -march=rv64i $ -ltr filename.o

![assem code](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/7eca9956-7668-4dc6-8e9f-4392d6b66da9)

![assem2 code](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/35420d5f-c3b3-4548-bc35-e8a96b4c155c)

By displaying the result in the less editor, this makes navigating easier. To find the keyword main, we use?main.

![Ofast](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/ad8f7181-1939-4949-b475-bdb70f1bf118)

RCV64-unknown-elf-gcc-Ofast -mabi=lp64 -march=rv64i -o filename.o filename are the guidelines for analyzing assembly code.b Employ $ riscv64-unknown-elf-objdump -d filename.o | less /main

![Ofast 2](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/97e1425f-565e-4f26-bd93-cf7b47175bfb)

We will tally the number of instructions that are carried out in the main block by using a hexadecimal calculator and subtracting the address numbers given at the left end. There are fifteen lines in the main block of instructions. Let's take a different method with the code compilation. -Ofast ought to be utilized rather than -O1.

![final output](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/c692c601-9f40-44e0-b6b4-40e6a84a7d81)

Simulation: This program simulates a clock divider in software. In a real hardware implementation, you would use a hardware description language (HDL) like Verilog or VHDL to design the clock divider circuit.

Flexibility: You can change the divisor and cycles values to simulate different clock division scenarios.

Environment: The instructions assume a development environment set up for RISC-V-cross-compilation.


# TASK 3

Run the RISC-V Objdmp in conjunction with SPIKE Simulation and Verification using -O1 and -Ofast.


We must use the (-o1) and (-ofast) commands to watch Spike Simulation in this work.

The C code may be proved to function on both a kit and a chip by compiling it in both RISCV and GCC. The clock divider's overall reliability and performance are improved by accurately implementing the project's C code, cutting down on development time, and minimizing human error through the use of an AI tool that generates the clock divided output.

![Spike simulation](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/9a8c5e06-f0da-40fb-822b-9cac3c9834c3)

Using a new tab, open your project's assembly code and type the following command to inspect it before beginning debugging.

$ riscv64-unknown-elf-objdump -d clkdiv.o | less

![debug](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/0605560e-87da-48c7-986f-c82dbb6fec35)

Enter the following command as indicated to begin debugging the assembly code.

$ spike -d pk clkdiv.o

(spike) //

![output (2)](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/1f880267-979b-48dd-9253-71122a9619b7)

To input a command that will cause all instructions preceding that address to be run in order to debug the instruction that has to be done.

![output 3](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/b1bd2653-8955-4ed8-95ac-c97794b924cf)

The contents of the stack pointer can also be seen as indicated below, both before and after that instruction is executed.To see the next important instruction, keep hitting ENTER in a same manner.

![final op](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/fc2c3abe-78a0-49c6-acf4-1c40bcf6fd19)

# TASK 4

**Identify various RISC-V instruction type (R, I, S, B, U, J) and exact 32-bit instruction code in the instruction type format for below RISC-V instructions**

**ADD r6, r2, r1 SUB r7, r1, r2 AND r8, r1, r3 OR r9, r2, r5 XOR r10, r1, r4 SLT r11, r2, r4 ADDI r12, r4, 5 SW r3, r1, 2 SRL r16, r14, r2 BNE r0, r1, 20 BEQ r0, r0, 15 LW r13, r1, 2 SLL r15, r1, r2**

**Upload the 32-bit pattern on Github**

To provide you with the exact 32-bit instruction codes for each of the given RISC-V instructions, let's break down each instruction into its respective components and then determine the 32-bit machine code based on the RISC-V instruction format.

### R-Type Instructions

1. **ADD r6, r2, r1**
   - opcode: `0110011`
   - funct3: `000`
   - funct7: `0000000`
   - rs1: `r1` (00001)
   - rs2: `r2` (00010)
   - rd: `r6` (00110)
   - Machine Code: `0000000 00010 00001 000 00110 0110011`

2. **SUB r7, r1, r2**
   - opcode: `0110011`
   - funct3: `000`
   - funct7: `0100000`
   - rs1: `r1` (00001)
   - rs2: `r2` (00010)
   - rd: `r7` (00111)
   - Machine Code: `0100000 00010 00001 000 00111 0110011`

3. **AND r8, r1, r3**
   - opcode: `0110011`
   - funct3: `111`
   - funct7: `0000000`
   - rs1: `r1` (00001)
   - rs2: `r3` (00011)
   - rd: `r8` (01000)
   - Machine Code: `0000000 00011 00001 111 01000 0110011`

4. **OR r9, r2, r5**
   - opcode: `0110011`
   - funct3: `110`
   - funct7: `0000000`
   - rs1: `r2` (00010)
   - rs2: `r5` (00101)
   - rd: `r9` (01001)
   - Machine Code: `0000000 00101 00010 110 01001 0110011`

5. **XOR r10, r1, r4**
   - opcode: `0110011`
   - funct3: `100`
   - funct7: `0000000`
   - rs1: `r1` (00001)
   - rs2: `r4` (00100)
   - rd: `r10` (01010)
   - Machine Code: `0000000 00100 00001 100 01010 0110011`

6. **SLT r11, r2, r4**
   - opcode: `0110011`
   - funct3: `010`
   - funct7: `0000000`
   - rs1: `r2` (00010)
   - rs2: `r4` (00100)
   - rd: `r11` (01011)
   - Machine Code: `0000000 00100 00010 010 01011 0110011`

### I-Type Instructions

1. **ADDI r12, r4, 5**
   - opcode: `0010011`
   - funct3: `000`
   - rs1: `r4` (00100)
   - rd: `r12` (01100)
   - imm: `000000000101`
   - Machine Code: `000000000101 00100 000 01100 0010011`

2. **LW r13, r1, 2**
   - opcode: `0000011`
   - funct3: `010`
   - rs1: `r1` (00001)
   - rd: `r13` (01101)
   - imm: `000000000010`
   - Machine Code: `000000000010 00001 010 01101 0000011`

### S-Type Instructions

1. **SW r3, r1, 2**
   - opcode: `0100011`
   - funct3: `010`
   - rs1: `r1` (00001)
   - rs2: `r3` (00011)
   - imm: `000000000010`
   - Machine Code: `0000000 00011 00001 010 00010 0100011`

### B-Type Instructions

1. **BNE r0, r1, 20**
   - opcode: `1100011`
   - funct3: `001`
   - rs1: `r0` (00000)
   - rs2: `r1` (00001)
   - imm: `000000010100` (20)
   - Machine Code: `0000000 00001 00000 001 01000 1100011`

2. **BEQ r0, r0, 15**
   - opcode: `1100011`
   - funct3: `000`
   - rs1: `r0` (00000)
   - rs2: `r0` (00000)
   - imm: `000000001111` (15)
   - Machine Code: `0000000 00000 00000 000 01111 1100011`

### R-Type Instructions (continued)

1. **SRL r16, r14, r2**
   - opcode: `0110011`
   - funct3: `101`
   - funct7: `0000000`
   - rs1: `r14` (01110)
   - rs2: `r2` (00010)
   - rd: `r16` (10000)
   - Machine Code: `0000000 00010 01110 101 10000 0110011`

2. **SLL r15, r1, r2**
   - opcode: `0110011`
   - funct3: `001`
   - funct7: `0000000`
   - rs1: `r1` (00001)
   - rs2: `r2` (00010)
   - rd: `r15` (01111)
   - Machine Code: `0000000 00010 00001 001 01111 0110011`



```plaintext
# RISC-V 32-bit Instruction Codes

ADD r6, r2, r1: 0000000 00010 00001 000 00110 0110011
SUB r7, r1, r2: 0100000 00010 00001 000 00111 0110011
AND r8, r1, r3: 0000000 00011 00001 111 01000 0110011
OR r9, r2, r5: 0000000 00101 00010 110 01001 0110011
XOR r10, r1, r4: 0000000 00100 00001 100 01010 0110011
SLT r11, r2, r4: 0000000 00100 00010 010 01011 0110011
ADDI r12, r4, 5: 000000000101 00100 000 01100 0010011
SW r3, r1, 2: 0000000 00011 00001 010 00010 0100011
SRL r16, r14, r2: 0000000 00010 01110 101 10000 0110011
BNE r0, r1, 20: 0000000 00001 00000 001 01000 1100011
BEQ r0, r0, 15: 0000000 00000 00000 000 01111 1100011
LW r13, r1, 2: 000000000010 00001 010 01101 0000011
SLL r15, r1, r2: 0000000 00010 00001 001 01111 0110011
```





































 

 
 


 



