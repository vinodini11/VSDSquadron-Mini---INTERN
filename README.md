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




 

 
 


 



