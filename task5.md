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
![309699508-ba781b31-81bb-4003-9b93-cff8f7825d9a](https://github.com/1165111981/apeksha/assets/160841230/5f3ef9fc-8188-450f-8aca-d6f5cd13401a)


## 3. INSTRUCTION SET OF RISC-V RV32I
![309703119-9b986703-34be-4527-8558-1e2cea21f4f9](https://github.com/1165111981/apeksha/assets/160841230/b04845c4-0239-42d8-8a4c-4ed429bddff6)

![309703267-0b2e2308-186c-4f70-9081-54ff8b3190ca](https://github.com/1165111981/apeksha/assets/160841230/b475398a-5eb1-4446-8865-7f014acae5a9)


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
```
![t53](https://github.com/1165111981/apeksha/assets/160841230/17fca56e-93c3-4203-97bb-b4fdd253eeb6)
- **To see the output waveform in gtkwave, enter the following commands in your terminal.**

`$ gtkwave hello.vcd`
![t55](https://github.com/1165111981/apeksha/assets/160841230/8eadc456-7527-450c-b8be-994a7dba3176)

### 4.3 The output waveform

The output waveform showing the instructions performed in a 5-stage pipelined architecture.
 
Instruction 1:add r6,r2,r1
 
<img width="1282" alt="309717644-9475de20-c117-476a-bebc-54dd3548c109" src="https://github.com/1165111981/apeksha/assets/160841230/4f236c24-70ce-450b-a5c6-85736f88c3b4">

Instruction 2:sub r7,r1,r2
<img width="1280" alt="309717941-2c95f18f-191e-4500-9cda-e7e838d1e609" src="https://github.com/1165111981/apeksha/assets/160841230/89a59cd0-0e5c-42ac-8308-0461cf55eef3">

Instruction 3:and r8,r1,r3
<img width="1282" alt="309718134-18bfdf76-1173-4984-b50b-83443ab48596" src="https://github.com/1165111981/apeksha/assets/160841230/7f7034e9-61a8-46d3-8883-998a961d7192">


Instruction 4:or r9,r2,r5
<img width="1294" alt="309718310-4f214bb2-c934-4778-bf46-841efe877fb8" src="https://github.com/1165111981/apeksha/assets/160841230/c818113f-2042-4d25-b1c9-31eb9b25656b">

Instruction 5:xor r10,r1,r4
<img width="1293" alt="309718453-6fa91f49-5e73-4133-8bf6-84ec4aca64da" src="https://github.com/1165111981/apeksha/assets/160841230/c7519520-c341-4fbb-aa6f-cf540788c708">


Instruction 6:slt r11,r2,r4
<img width="1290" alt="309718574-c9c32048-62ed-4f55-8e11-9763816b1bd1" src="https://github.com/1165111981/apeksha/assets/160841230/f1c47b44-feea-4c56-bc38-9c14afcfebac">


Instruction 7:addi r12,r4,5
<img width="1285" alt="309718717-308b8a9d-46c8-4a0e-8824-90e11d9a6a1e" src="https://github.com/1165111981/apeksha/assets/160841230/d4d3f486-f774-4542-a22f-5aa2548f2545">

Instruction 8:sw r3,r1,2
<img width="1280" alt="309718858-84f16d7f-9d16-4236-b64d-615e187a00ff" src="https://github.com/1165111981/apeksha/assets/160841230/8402187c-9a3d-499a-9f63-2750dce0c47b">

Instruction 9:lw r13,r1,2
<img width="1295" alt="309719046-c7bc7d9a-6745-4eeb-903d-fa723dca1394" src="https://github.com/1165111981/apeksha/assets/160841230/0e136141-4e46-4f3a-abbe-2e20b6ee270c">

Instruction 10:beq r0,r0,15
<img width="1287" alt="309719144-a1c6781f-c301-45d9-a502-fb32e6204e4c" src="https://github.com/1165111981/apeksha/assets/160841230/d513d07d-4d94-4ad8-9aba-209b097cf42d">

After branching, performing
<img width="1287" alt="309719297-56b50ce0-60aa-41fe-8f53-0b4583b39665" src="https://github.com/1165111981/apeksha/assets/160841230/296519a8-b0c9-4b58-a2a3-f28d96bec246">

Full 5-stage instruction pipeline and pc-increment description Waveform
  
<img width="1325" alt="309719447-e5ebc923-ad2c-44fc-a577-3ce7b8419bce" src="https://github.com/1165111981/apeksha/assets/160841230/e68a6a58-6861-4620-89dd-a455d7891cb7">

![t56](https://github.com/1165111981/apeksha/assets/160841230/963eb3db-3714-4c4e-8ed5-055ef307c70e)
![t57](https://github.com/1165111981/apeksha/assets/160841230/9674be64-a333-40eb-b097-f2325ceb9096)
![t58](https://github.com/1165111981/apeksha/assets/160841230/459d45d1-76e3-4322-904b-b1278b4a1248)
