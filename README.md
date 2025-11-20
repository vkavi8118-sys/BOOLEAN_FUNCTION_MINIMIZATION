# BOOLEAN_FUNCTION_MINIMIZATION

DATE:19.11.2025

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

module ex2 (a,b,c,d,w,x,y,z,f1,f2);

input a,b,c,d,w,x,y,z;

output f1,f2;

assign f1=~a&~b&~c&~d | a&~c&~d | ~b&c&~d | ~a&b&c&d | b&~c&d;

assign f2=x&~y&z | ~x&~y&z | ~w&x&y | w&~x&y | w&x&y;

endmodule

Developed by:Kavinaya V RegisterNumber:25017974


**RTL realization output**
<img width="1920" height="1080" alt="Screenshot (73)" src="https://github.com/user-attachments/assets/477d63a4-0df3-41a6-997c-812651a686c4" />

**Timing Diagram**
<img width="1920" height="1080" alt="Screenshot (74)" src="https://github.com/user-attachments/assets/531f1113-8236-454b-bb36-3d5c40ae986c" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

