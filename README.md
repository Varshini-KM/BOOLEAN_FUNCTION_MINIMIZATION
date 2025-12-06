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

Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 
```
module funct1(a,b,c,d,f1);
input a,b,c,d;
output f1;
assign f1=((~a & ~b & ~c & ~d)|(a & ~c & ~d)|(~b & c & ~d)|(b & ~c & d));
endmodule

module funct2(w,x,y,z,f2);
input w,x,y,z;
output f2;
assign f2=((x & ~y & z)|(~x & ~y & z)|( ~w & x & y)|(w & ~x & y)|(w & x & y));
endmodule
```

Developed by: RegisterNumber: 25018756



**RTL realization:**



F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/fad87da1-afef-4393-803a-a89e76136694" />


F2=xy’z+x’y’z+w’xy+wx’y+wxy

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1d0cc3c0-64b9-4de8-8a40-01acd48d7681" />





**Output(Timing Diagram RTL):**



F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/b42adff9-651f-4ab1-8488-ccb1ab0a00b9" />



F2=xy’z+x’y’z+w’xy+wx’y+wxy


<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/f7c667c1-b139-4e9a-9206-e4c5e6fc3b70" />




**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.




