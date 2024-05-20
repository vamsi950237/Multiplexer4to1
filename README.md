**AIM: **

To simulate and synthesis of Multiplexer4to1 using vivado 2023.2 

**APPARATUS REQUIRED:**

vivado 2023 

**PROCEDURE:** 

STEP:1 Start the vivado software, Select and Name the New project. 

STEP:2 Select the device family, device, package and speed. 

STEP:3 Select new source in the New Project and select Verilog Module as the Source 
type. 

STEP:4 Type the File Name and module name and Click Next and then finish button. 

Type the code and save it. 

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source 
Window and click the check syntax. 

STEP:6 Click the simulation to simulate the program and give the inputs and verify 
the outputs as per the truth table. 

STEP:7 compare the output with truth table. 

# Multiplexer4to1

# Truth Table
![image](https://github.com/RESMIRNAIR/Multiplexer4to1/assets/154305926/f1dac9e1-e938-4072-bfa9-c17a0a54b7c7)

# Circuit Diagram
![image](https://github.com/RESMIRNAIR/Multiplexer4to1/assets/154305926/f8ea8610-f6fc-4de3-a68a-5a9a4cfcd673)

**verilog code**

module mux(a,b,d,y);

input a,b;

input [3:0]d;

output y;

wire w1,w2,w3,w4;

assign w1=~a&~b&d[0];

assign w2=~a&b&d[1];

assign w3=~a&~b&d[2];

assign w4=a&b&d[3];

assign y=w1|w2|w3|w4;

endmodule

**output**

![muxhdl](https://github.com/nithin2134/Multiplexer4to1/assets/160302970/078298b2-3e1a-444b-971e-77b7757bec99)

**Result**
Thus the simulation and synthesis of Multiplexer4to1 using vivado 2023.2 is successfully executed and verified.




