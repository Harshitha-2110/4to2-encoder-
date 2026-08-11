# 4to2-encoder-
4-to-2 Encoder – Verilog

Description

A 4-to-2 encoder converts one of four active input signals into a corresponding 2-bit binary output.

Working

The encoder has 4 inputs (D3, D2, D1, D0) and 2 outputs (Y1, Y0).

Active Input| Y1| Y0
D0| 0| 0
D1| 0| 1
D2| 1| 0
D3| 1| 1

«Note: Only one input should be HIGH at a time.»

 Project Structure

4to2-encoder/
├── README.md
├── encoder_4to2.v
└── tb_encoder_4to2.v

Tools

- Verilog HDL
- Icarus Verilog
- GTKWave

 Simulation

Compile the design and testbench:

iverilog -o encoder_sim encoder_4to2.v tb_encoder_4to2.v

Run the simulation:

vvp encoder_sim

Generate a waveform:

gtkwave encoder_4to2.vcd

Expected Output

D3 D2 D1 D0 | Y1 Y0
------------|------
0  0  0  1  | 0  0
0  0  1  0  | 0  1
0  1  0  0  | 1  0
1  0  0  0  | 1  1

 Applications

- Digital logic circuits
- Data encoding
- Communication systems
- Digital control systems
- Processor and memory systems
author: Harshitha 