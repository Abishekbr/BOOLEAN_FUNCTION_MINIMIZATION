# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

A combinational circuit is a circuit in which the output depends on the present combination of inputs. Combinational circuits are made up of logic gates. The output of each logic gate is determined by its logic function. Combinational circuits can be made using various logic gates, such as AND gates, OR gates, and NOT gates.

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


## Program:
```
Developed by: B.R.Abishek
RegisterNumber:212224110002
```
```
module combinationalcircuit(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule
```


## RTL realization:


![311433218-f0108d3e-78c4-49fa-9661-c9d5bbf2b99b](https://github.com/23004513/BOOLEAN_FUNCTION_MINIMIZATION/assets/138973069/ccd61b61-3b31-4260-8be8-3d14def18992)


## Truth Table:

![311433313-399f99d5-79cc-443a-b54a-41d7a0326a5c](https://github.com/23004513/BOOLEAN_FUNCTION_MINIMIZATION/assets/138973069/9439745f-7933-4186-b5ae-efcce4c473a1)


## Timing Diagram:
![de](https://github.com/Prasannalakshmiganesan/BOOLEAN_FUNCTION_MINIMIZATION/assets/118610231/fbc7926d-3ba1-44fd-9483-fc1aa2d8d2d0)



## Result:

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.
