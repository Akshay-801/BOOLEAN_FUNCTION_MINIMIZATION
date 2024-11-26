# BOOLEAN_FUNCTION_MINIMIZATION

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

Developed by: AKSHAY M
RegisterNumber: 24900489

```
module Bool_min(A,B,C,D,W,X,Y,Z,F1,F2);
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

**Logic symbol & Truthtable**

![Screenshot 2024-11-26 162123](https://github.com/user-attachments/assets/49a7e8cb-a212-4483-b59d-ba34b51ee94c)

![Screenshot 2024-11-26 162156](https://github.com/user-attachments/assets/36be79c0-9aef-4743-8f01-4f43478eaa2b)


**RTL realization**

![Screenshot 2024-11-26 162227](https://github.com/user-attachments/assets/43f253ef-8aa6-4cc1-82ca-464ea33629d0)


**RTL**

![rtl](https://github.com/user-attachments/assets/b4a25e8b-8a97-45b8-a164-62489bf99c89)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

