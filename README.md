# BOOLEAN_FUNCTION_MINIMIZATION
```
Developed by Srikanth K
Register Number: 25017937
```
**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module Boolean_min(A,B,C,D,W,X,Y,Z,F1,F2);
input A,B,C,D,W,X,Y,Z;
wire x1,x2,x3,x4,x5,x6,x7,x8,x9,x10;
output F1,F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(~W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

```
**Logic symbol & Truthtable:**
<img width="805" height="442" alt="image" src="https://github.com/user-attachments/assets/9f87e18e-6a17-4efa-8be6-100dc1a3293c" />
<img width="797" height="421" alt="image" src="https://github.com/user-attachments/assets/5bd233f7-9ed4-4248-a490-8273563ed85c" />



**RTL realization**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/33cc38f7-4a39-4c90-adca-f8819e87e0b1" />

**Output:**
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/66f020c4-7b23-48e9-b1fa-894ba91c1d38" />



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

