# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
```
## Hardware – PCs, Cyclone II , USB flasher
## Software – Quartus prime
```

## Theory
 

## Logic Diagram
## Procedure
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: saridha M A
RegisterNumber: 23013627  
*/
```
module ex2(A,B,C,D,F1);
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
## RTL realization

![image](https://github.com/sandhiya2815/Experiment--02-Implementation-of-combinational-logic-/assets/155123230/9974a5f1-2113-47f7-a5fe-2b02b149a8bd)

## Truth Table
![image](https://github.com/sandhiya2815/Experiment--02-Implementation-of-combinational-logic-/assets/155123230/56c5889f-e19e-41ae-a030-ba794754cd74)

## Timing Diagram
![image](https://github.com/sandhiya2815/Experiment--02-Implementation-of-combinational-logic-/assets/155123230/4a7687a4-b839-40ae-813d-021afc206de4)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
