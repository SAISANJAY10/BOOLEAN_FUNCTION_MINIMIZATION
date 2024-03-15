**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
Developed by:SAI SANJAY R 

RegisterNumber:212223040178

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module exp22(A,B,C,D,F1);
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

**LOGIC DIAGRAM**
![Screenshot 2024-03-15 111842](https://github.com/SAISANJAY10/BOOLEAN_FUNCTION_MINIMIZATION/assets/144228073/e6ac351a-59a5-4a58-a95c-07eafd16392f)

**RTL REALIZATION**
![Screenshot 2024-03-15 111901](https://github.com/SAISANJAY10/BOOLEAN_FUNCTION_MINIMIZATION/assets/144228073/d7eca012-11a1-4ed8-be63-a85152f95f3e)

**OUTPUT: TRUTH TABLE**
![Screenshot 2024-03-15 111921](https://github.com/SAISANJAY10/BOOLEAN_FUNCTION_MINIMIZATION/assets/144228073/1bbc5095-a40c-485a-a14b-e56b99720ab6)


**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

