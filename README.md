# ALU
Company: CODTECH IT SOLUTIONS

Name: Pooja Shukla

Intern ID: CT06DH677

Domain: VLSI

Duration: 6 weeks

Mentor Name: Neela Santosh

##In this project, I designed a simple Arithmetic Logic Unit (ALU) using Verilog code and simulated it on the EDA Playground. The ALU is a fundamental combinational circuit in the VLSI domain that performs various arithmetic and logical operations on input operands based on control signals.
Design Code Overview

The ALU design module accepts two 4-bit inputs, A and B, and a 3-bit select signal sel to choose the operation. The output is an 5-bit result. The operations implemented in the ALU include:

Addition (sel=000)

Subtraction (sel=001)

Multiplication operation (sel=010)

Division operation (sel=011)

Modulo-division operation (sel=100)

And operation (sel=101)

Or operation (sel=110)

Not operation (sel=111)


The ALU code uses a case statement to map select signals to specific operations, ensuring clean, readable, and synthesizable design logic.

Testbench Overview

The testbench module instantiates the ALU design and applies various input combinations to validate all functionalities. The inputs A, B, and sel are declared as reg type, and output out is declared as wire type. In the testbench, an initial block is used to assign values to inputs sequentially with time delays (#1) for clear observation of each operation in the simulation.


$monitor is used for console output of input, select, and output values at each time instant during simulation, enabling easy verification.

Simulation in EDA Playground

The design and testbench were simulated using the aldec Verilog simulator on the EDA Playground platform. The simulation results were observed, verifying that:

Addition operation produced correct results.

Subtraction operation handled signed results properly.

Logical operations performed bitwise calculations accurately.



EDA Playground provided an online collaborative environment where design and testbench were placed in separate tabs, with design.sv containing the ALU module and testbench.sv containing the stimulus code. The platform facilitated quick debugging, waveform viewing, and version-controlled sharing with peers or faculty.

Importance in VLSI Domain

ALU design is a crucial building block in datapath design of processors. Understanding its Verilog implementation strengthens concepts in RTL coding, module instantiation, case-based operation control, and simulation analysis, which are essential skills for VLSI front-end design roles in the semiconductor industry.
