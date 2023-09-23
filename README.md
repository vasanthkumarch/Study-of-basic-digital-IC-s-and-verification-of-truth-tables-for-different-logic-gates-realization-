# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime


## Theory
 

## Logic Diagram
## Procedure
## Program:
```
module DE_EX_02(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(~A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1= x1|x2|x3|x4|x5;
endmodule
/*
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
# Developed by: R.Vignesh
# RegisterNumber:212222230172  
*/
## Output:
## RTL
![image](https://github.com/Udhayasankaran04/Experiment--02-Implementation-of-combinational-logic-/assets/119393933/fc756bcc-a442-4611-bb9a-aed46d7bd6bb)

## Timing Diagram
 ![image](https://github.com/Udhayasankaran04/Experiment--02-Implementation-of-combinational-logic-/assets/119393933/11fc3782-a1c8-41f8-a174-af542fe709cc)

## TRUTH TABLE
![image](https://github.com/Udhayasankaran04/Experiment--02-Implementation-of-combinational-logic-/assets/119393933/57c5ce60-e1ff-4ec6-bcf0-24f38c7661c5)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
