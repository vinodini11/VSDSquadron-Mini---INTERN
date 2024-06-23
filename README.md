# VSDSquadron Mini-INTERN
DESCRIPTION:

A development board for RISC-V is the vsdsquadron mini. A 32-bit RISC-V core resides within it. It runs on a 24MHz frequency and contains 16KB of flash memory and 2KB of SRAM. Supporting protocols including SPI, USART, and I2C, the board contains fifteen GPIO pins.

PROCESS:

The tasks at hand include installing Ubuntu on VMBox, Visual C++, and writing an example of C code along with analyzing RISC assembly code for the sample C code. These are the essential programs for this internship.

Installing Ubuntu on VMBox Open the Ubuntu terminal after installing the tools, then type the command.


Order for Installation of Leafpad apt-get install leafpad $ sudo

 $ cd $ leafpad filename.c & to launch Leafpad

 ![To Open Leafpad](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/5ac9fcc7-2363-4219-ad11-a9aa96f3ba2a)

 PROGRAM:
 To Find the Sum Of Product

 ![TO FIND THE SUM PROGRAM](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/340df625-8b93-41f0-9fc6-7dbd6e40cea2)

 ![PROGRAM](https://github.com/vinodini11/VSDSquadron-Mini-INTERN/assets/173384059/094195cd-567e-46d8-9f0e-b532b6093524)

 The Output for the Program

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





 

 
 


 



