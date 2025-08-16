4-bit Full Adder Design using IP Catalog in Xilinx Vivado

📌 Project Overview
This project demonstrates the design and implementation of a 4-bit Full Adder using the IP Catalog in Xilinx Vivado. The design leverages pre-built IP cores (Adder/Subtractor) to implement arithmetic logic instead of manually coding the RTL. This approach highlights the benefits of using Vivado’s IP Integrator for quick prototyping and modular hardware design.
The 4-bit Full Adder takes two 4-bit binary inputs along with a carry-in and produces a 4-bit sum along with a carry-out.

⚙️ Features
Implemented using Vivado IP Catalog (Adder/Subtractor IP)
4-bit addition with carry-in and carry-out
Synthesizable design suitable for FPGA implementation
Easy to extend for larger bit-widths
Testbench provided for functional verification

🧩 Design Details

Inputs:
A[3:0] : 4-bit input operand
B[3:0] : 4-bit input operand
Cin : Carry-in (1-bit)

Outputs:
SUM[3:0] : 4-bit sum output
Cout : Carry-out (1-bit)

Vivado Components Used:
Adder/Subtractor IP core
IP Integrator (Block Design)

├── src/                  # Source files (Vivado Block Design, HDL Wrappers)
├── sim/                  # Testbench files
├── constraints/          # XDC constraint file (if mapped to FPGA)
├── docs/                 # Screenshots, block diagrams
├── results/              # Simulation results
└── README.md             # Project documentation

▶️ How to Run
Open Xilinx Vivado (2020.2 or later recommended).
Create a new project → Add source files.
Use IP Catalog to generate the Adder/Subtractor IP.
Configure IP for 4-bit addition with carry-in.
Integrate IP into Block Design.
Generate HDL wrapper and run synthesis/implementation.
Use testbench (sim/) to verify functionality.

📊 Simulation Result
Verified correct 4-bit addition with carry propagation.
Functional waveform shows expected outputs for different input combinations.

🚀 Future Enhancements
Extend to 8-bit or 16-bit Adder
Integrate with ALU design
Add Subtraction functionality using IP configuration

🛠️ Tools Used
Xilinx Vivado Design Suite (IP Catalog, Simulation, Synthesis)
ModelSim / Vivado Simulator for verification
GitHub for version control and documentation

Acknowledgments
||=>xilinx Vivado documentation for IP core creation.
||=>Verilog HDL reference for full adder design.
