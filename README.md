# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime


## Theory:
Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.

Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output. F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

1.AND gate The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB Y= A.B

2.OR gate The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation. Y= A+B
 

## Logic Diagram
## Procedure
## Program:
```
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: yuva krishna k
RegisterNumber:  212222110056
```
```
module f1(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire p,q,r,s,t;
assign p = (~A & ~B & ~C & ~D);
assign q = (A & ~C & ~D);
assign r = (~B & C & ~D);
assign s = (~A & B & C & D);
assign t = (B & ~C & D);
assign F1 = p | q | r | s | t;
endmodule
```
## RTL realization:
![266632555-15b89c9c-a933-49a4-b0c3-10750cbfb703](https://github.com/Yuvakrishna0/Experiment--02-Implementation-of-combinational-logic-/assets/117915037/ff3440e7-9c68-4eb9-a93c-666eed27abd3)

## Truthtable:
![266632975-18913584-a8b8-4898-a37c-9acfcb428604](https://github.com/Yuvakrishna0/Experiment--02-Implementation-of-combinational-logic-/assets/117915037/44de15ae-7604-4c6d-8f55-d184440c9921)

## Output:

![266632733-93add01e-4113-43f5-8857-b24398c362be](https://github.com/Yuvakrishna0/Experiment--02-Implementation-of-combinational-logic-/assets/117915037/5febac7f-4a93-43b0-ad9b-0ed56471b187)


## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
