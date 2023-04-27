# Experiment--02-Implementation-of-combinational-logic
Implementation of combinational logic gates
 
## AIM:
To implement the given logic function verify its operation in Quartus using Verilog programming.
 F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D
F2=xy’z+x’y’z+w’xy+wx’y+wxy
 
 
 
## Equipments Required:
 Hardware – PCs, Cyclone II , USB flasher
 Software – Quartus prime


## Theory
 Logic gates are electronic circuits which perform logical functions on one or more inputs to produce one output.
## Using NAND gates:
   NAND gate is actually a combination of two logic gates i.e. AND gate followed by NOT gate. So its output is complement of the output of an AND gate.This gate can have minimum two inputs, output is always one. By using only NAND gates, we can realize all logic functions: AND, OR, NOT, X-OR, X-NOR, NOR. So this gate is also called as universal gate. First note that the entire expression is inverted and we have three terms ANDed. This means that we must use a 3-input NAND gate. Each of the three terms is, itself, a NAND expression. Finally, negated single terms can be generates with a 2-input NAND gate acting as an inverted.

F=((C'.B.A)'(D'.C.A)'(C.B'.A)')'
## Using NOR gates:
   NOR gate is actually a combination of two logic gates: OR gate followed by NOT gate. So its output is complement of the output of an OR gate. This gate can have minimum two inputs, output is always one. By using only NOR gates, we can realize all logic functions: AND, OR, NOT, Ex-OR, Ex-NOR, NAND. So this gate is also called universal gate. Designing a circuit with NOR gates only uses the same basic techniques as designing a circuit with NAND gates; that is, the application of deMorgan’s theorem. The only difference between NOR gate design and NAND gate design is that the former must eliminate product terms and the later must eliminate sum terms.

F=(((C.B'.A)+(D.C'.A)+(C.B'.A))')'
## Procedure:
```
1.Create a project with required entities. 
2.Create a module along with respective file name.
3.Run the respective programs for the given boolean equations. 
4.Run the module and get the respective RTL outputs.
5.Create university program(VWF) for getting timing diagram. 
6.Give the respective inputs for timing diagram and obtain the results.
```
## Program:
/*
Program to implement the given logic function and to verify its operations in quartus using Verilog programming.
Developed by: Kavinesh M
RegisterNumber:212222230064  
*/
## RTL realization

## Output:
## Using NAND:
## RTL
![crtl1](https://user-images.githubusercontent.com/118466561/234770092-caafa17a-d126-46a8-903e-7c809829aff4.png)
## Timing Diagram
![c1wf](https://user-images.githubusercontent.com/118466561/234770552-3123b328-c893-448a-8448-1e347a30f764.png)
## Truth Table
![image](https://user-images.githubusercontent.com/118466561/234770890-e6332bc7-f840-47fa-b2f1-c40654db6e95.png)
## Using NOR:
## RTL
![crtl2](https://user-images.githubusercontent.com/118466561/234771558-2da86a3a-1da2-4609-81ab-9deb71b4ad22.png)

## Timing Diagram
![c2wf](https://user-images.githubusercontent.com/118466561/234771592-3bdac7b4-9f1c-4053-ae80-e0dbe6e1b251.png)

## Truth Table
![image](https://user-images.githubusercontent.com/118466561/234771646-e13a292e-57ad-40bc-8307-d7029fd80548.png)

## Result:
Thus the given logic functions are implemented using  and their operations are verified using Verilog programming.
