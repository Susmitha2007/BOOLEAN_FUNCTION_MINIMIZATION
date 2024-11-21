![image](https://github.com/user-attachments/assets/6884df4b-4b6f-4302-9fe4-23aeaffed370)# BOOLEAN_FUNCTION_MINIMIZATION

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

Developed by:Nara Guna Susmitha RegisterNumber:24010204*/

```
module exp002(A, B, C, D, W, X, Y, Z, F1,F2);
input A, B, C, D,W,X,Y,Z;
wire x1, x2, x3, x4, x5, x6, x7, x8, x9, x10;
output F1, F2;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign x6=(X)&(~Y)&(Z);
assign x7=(~X)&(~Y)&(Z);
assign x8=(-W)&(X)&(Y);
assign x9=(W)&(~X)&(Y);
assign x10=(W)&(X)&(Y);
assign F1=x1|x2|x3|x4|x5;
assign F2=x6|x7|x8|x9|x10;
endmodule

```

**RTL realization**
![Screenshot 2024-11-21 214309](https://github.com/user-attachments/assets/26a6b4fb-6d1a-4977-b19e-294f47dacdad)

**Output:**
![WhatsApp Image 2024-11-21 at 9 39 00 PM](https://github.com/user-attachments/assets/4f1beb3e-3666-4771-a74c-27824b4d01de)

**RTL**
![Screenshot 2024-11-21 214422](https://github.com/user-attachments/assets/e50f66e0-e871-4904-9aff-be770893986a)

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

