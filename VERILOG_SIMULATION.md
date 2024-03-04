# As per the Update given for the next task "Should Use the RISC-V Core Verilog netlist and testbench for functional Simulation.
# Veriog code is being executed and the waveforms are generated using the gtkwave

# Aim: To verify the Functional Simulation:-
# Table of contents
- [1.RISC-V RV32I](#1-RISC-V-RV32I)
 - [2.BLOCK DIAGRAM OF RISC-V RV32I](#2-BLOCK-DIAGRAM-OF-RISC-V-RV32I)
 - [3.INSTRUCTION SET OF RISC-V RV32I](#3-INSTRUCTION-SET-OF-RISC-V-RV32I)
 - [4.FUNCTIONAL SIMULATION](#4-FUNCTIONAL-SIMULATION)
    - [4.1 About iverilog and gtkwave](#41-About-iverilog-and-gtkwave)
    - [4.2 Installing iverilog and gtkwave](#42-Installing-iverilog-and-gtkwave)
    - [4.3 The output waveform](#43-The-output-waveform)
  
   ## 1. RISC-V RV32I

This project provides an insight into the working of a few important instructions of the instruction set of a Single cycle Reduced Instruction Set Computer - Five(RISC-V) Instruction Set Architecture suitable for use across wide-spectrum of Applications from low-power embedded devices to high-performance Cloud-based Server processors. The base RISC-V is a 32-bit processor with 31 general-purpose registers, so all the instructions are 32-bit long. Some Applications where the RISC-V processors have begun to make some significant threads are in Artificial intelligence and machine learning, Embedded systems, ultra-low power processing systems, etc.

## 2. BLOCK DIAGRAM OF RISC-V RV32I
![image](https://github.com/1165111981/apeksha/assets/160841230/0f621e18-ec4f-4abe-b982-d8338dccac51)


## 3. INSTRUCTION SET OF RISC-V RV32I
![image](https://github.com/1165111981/apeksha/assets/160841230/1a9b9d51-e259-4edd-be0f-b506d837efbb)

![image](https://github.com/1165111981/apeksha/assets/160841230/ebcceb73-1003-4715-87d8-f94990404f0b)


## 4. FUNCTIONAL SIMULATION

### 4.1 About iverilog and gtkwave
- Icarus Verilog is an implementation of the Verilog hardware description language.
- GTKWave is a fully featured GTK+ v1. 2 based wave viewer for Unix and Win32 which reads Ver Structural Verilog Compiler generated AET files as well as standard Verilog VCD/EVCD files and allows their viewing.

### 4.2 Installing iverilog and gtkwave

- **For Ubuntu**

Open your terminal and type the following to install iverilog and GTKWave
 ```
$   sudo apt get update
$   sudo apt get install iverilog gtkwave
 ```

![t51](https://github.com/1165111981/apeksha/assets/160841230/86223f4d-bb7f-4a6b-a8a2-c8fda699f7dc)


- **To clone the repository and download the netlist files for simulation, enter the following commands in your terminal.**

 ```
$ git clone https://github.com/1165111981/apeksha.git
$ cd apeksha
```
![t52](https://github.com/1165111981/apeksha/assets/160841230/dee69508-86d7-456b-8edb-e0027e302807)
- **To simulate and run the Verilog code, enter the following commands in your terminal.**
```
$ iverilog -o hello hello.v hello_tb.v
$ ./hello
![t55](https://github.com/1165111981/apeksha/assets/160841230/2690978a-2370-4ad1-adf1-6f200004be19)
-**To see the output waveform in gtkwave, enter the following commands in your terminal.**
`$ gtkwave hello.vcd`
![t55](https://github.com/1165111981/apeksha/assets/160841230/42fec1aa-813c-4a1b-ab5d-1ab7a0784a11)
### 4.3 The output waveform
The output waveform showing the instructions performed in a 5-stage pipelined architecture.
Instruction 1:add r6,r2,r1
![image](https://github.com/1165111981/apeksha/assets/160841230/1873da9e-a56e-43d5-94a0-eac69fad8642)
Instruction 2:sub r7,r1,r2
![image](https://github.com/1165111981/apeksha/assets/160841230/4f2d5493-84e9-4dee-a86d-efd0afe4921d)
Instruction 3:and r8,r1,r3
![image](https://github.com/1165111981/apeksha/assets/160841230/3198f9d9-b9ad-46f6-aee5-c9c4a442a43f)
Instruction 4:or r9,r2,r5
![image](https://github.com/1165111981/apeksha/assets/160841230/e1843352-a429-4eab-ad68-91b2cbb2e681)
Instruction 5:xor r10,r1,r4
![image](https://github.com/1165111981/apeksha/assets/160841230/3532dc86-bf32-40c0-9f87-23d1ff703ac1)
Instruction 6:slt r11,r2,r4
![image](https://github.com/1165111981/apeksha/assets/160841230/b4d51014-bec1-4f34-8e39-76a02f160024)
Instruction 7:addi r12,r4,5
![image](https://github.com/1165111981/apeksha/assets/160841230/2644ed87-b0e3-45ed-8604-05162d3dabe5)
Instruction 8:sw r3,r1,2
![image](https://github.com/1165111981/apeksha/assets/160841230/6cd291bd-ce94-4c27-9e79-fb6a5b4789f4)
Instruction 9:lw r13,r1,2
<img width="1295" alt="309719046-c7bc7d9a-6745-4eeb-903d-fa723dca1394" src="https://github.com/1165111981/apeksha/assets/160841230/11fdc161-a393-4f2e-875c-47120b8d1b73">
Instruction 10:beq r0,r0,15
<img width="1287" alt="309719144-a1c6781f-c301-45d9-a502-fb32e6204e4c" src="https://github.com/1165111981/apeksha/assets/160841230/ea966e6e-1278-458c-afa9-47277b66f221">
After branching, performing
Instruction 11:add r14,r2,r2
<img width="1287" alt="309719297-56b50ce0-60aa-41fe-8f53-0b4583b39665" src="https://github.com/1165111981/apeksha/assets/160841230/5581705f-32f7-4b45-b124-1854463ca31d">
Full 5-stage instruction pipeline and pc-increment description Waveform
<img width="1325" alt="309719447-e5ebc923-ad2c-44fc-a577-3ce7b8419bce" src="https://github.com/1165111981/apeksha/assets/160841230/d4faa404-0d80-421a-9565-7b0ab5488829">
![t56](https://github.com/1165111981/apeksha/assets/160841230/b2450d55-e8b6-43b7-9ace-f487661c0c57)
![t57](https://github.com/1165111981/apeksha/assets/160841230/2eead6ba-5a9f-4b0c-a798-c508b8681c1e)
![t58](https://github.com/1165111981/apeksha/assets/160841230/1d5a93c2-84a3-4b2a-b8b5-d6a3c12c8a10)


