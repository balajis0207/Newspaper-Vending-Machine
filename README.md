📰 Newspaper Vending Machine using Verilog FSM
📌 Project Overview

This project implements a Finite State Machine (FSM) based Newspaper Vending Machine controller using Verilog HDL. The design models a real-world vending machine that accepts coins, tracks the total inserted amount, and dispenses a newspaper when the required amount is reached. The complete design is simulated and verified using Xilinx Vivado.

🎯 Design Specifications

Newspaper cost: 15 cents

Accepted coins:

Nickel (5¢) → 01

Dime (10¢) → 10

FSM Type: Moore Machine

Output: newspaper goes HIGH for one clock cycle when 15¢ is reached

Extra change: Not returned

Reset: Synchronous/Asynchronous (as per design)

🧠 FSM Architecture

The system is designed using a multi-state FSM:

State	Meaning
S0	0 cents inserted
S5	5 cents inserted
S10	10 cents inserted
S15	15 cents reached
DISP	Dispense newspaper

The FSM transitions between states based on coin inputs and ensures a glitch-free output pulse using Moore-style logic.

🧩 Design Files
📁 Newspaper-Vending-Machine-Verilog
 ├── vending_fsm.v        # FSM design (RTL)
 ├── tb_vending_fsm.v     # Testbench for simulation
 └── README.md

🧪 Simulation & Verification

Tool used: Xilinx Vivado

Simulation type: Behavioral Simulation

Verified correct FSM transitions and output pulse

Waveform confirms single-clock newspaper dispense signal

▶ How to Run in Vivado

Open Vivado

Create a new RTL Project

Add vending_fsm.v as Design Source

Add tb_vending_fsm.v as Simulation Source

Set testbench as top module

Run Behavioral Simulation

Observe waveform for newspaper output

🛠 Tools & Technologies

Verilog HDL

Xilinx Vivado

FSM (Moore Machine)

RTL Design Methodology

Digital Logic Design

📈 Learning Outcomes

Practical understanding of FSM-based controllers

Clean separation of combinational and sequential logic

RTL coding best practices

Simulation-driven verification

FPGA-ready design flow

🚀 Future Enhancements

Add change return logic

Implement FPGA board (Basys-3 / Artix-7)

Add coin sensor interface

Extend FSM for multiple products

👤 Author

S Balaji
Electronics / VLSI Enthusiast
Verilog | FPGA | Digital Design
