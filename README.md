# T_FLIPFLOP
# AIM
To simulate and synthesis T flipflop using vivado.
# APPARATUS REQUIRE
Vivado 2023.2 software.
# pROCEDURE
STEP:1 Start the vivado software, Select and Name the New project.

STEP:2 Select the device family, device, package and speed.

STEP:3 Select new source in the New Project and select Verilog Module as the Source type.

STEP:4 Type the File Name and module name and Click Next and then finish button. Type the code and save it.

STEP:5 Select the run simulation and then run Behavioral Simulation in the Source Window and click the check syntax.

STEP:6 Click the simulation to simulate the program and give the inputs and verify the outputs as per the truth table.

STEP:7 compare the output with truth table.
# CIRCUIT DIAGRAM
![image](https://github.com/kanipakajeevana/T_FLIPFLOP/assets/170450203/843c2005-be5f-435b-8f4b-7ce9c28fb8ac)
# TRUTH TABLE
![image](https://github.com/kanipakajeevana/T_FLIPFLOP/assets/170450203/6b9d5d3e-98ef-4da8-9f03-d55eb748b0a4)
# PROGRAM
module tff(clk,reset,t,q);
input clk,reset,t;
output reg q;
always @(posedge clk
begin
if(reset==1)
q=0;
else
begin
if(t==0)
q=q;
else
q=~q;
end
end
endmodule
# OUTPUT
![image](https://github.com/kanipakajeevana/T_FLIPFLOP/assets/170450203/ec46a80c-e18f-43bf-b886-8ba4eaab0953)
# RESULT
Thus the verilog program for T flipflop has been simulated and verified successfully.




