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
```
F(A,B,C,D)=AB+CD+AD

module boolean_function_4var (
    input  wire A,
    input  wire B,
    input  wire C,
    input  wire D,
    output wire F
);

assign F = (~A & B) | (C & D) | (A & ~D);

endmodule

module funct2(w,x,y,z,f2);

input w,x,y,z;

output f2;

assign f2=((~y & z)|( w & y )|(x & y));

endmodule
```
Developed by: RegisterNumber:*/


**RTL realization**
<img width="1907" height="974" alt="Screenshot 2025-11-23 214239" src="https://github.com/user-attachments/assets/ba24e913-dcfa-4d3d-8fd7-72abdc4e122f" />
<img width="1635" height="930" alt="Screenshot 2025-11-23 220448" src="https://github.com/user-attachments/assets/6c38fac4-a663-4fe8-97e6-9442a4e6b45d" />
**Output:**

**RTL**

**Timing Diagram**
<img width="1907" height="977" alt="Screenshot 2025-11-23 193520" src="https://github.com/user-attachments/assets/d7fbd82a-8cf9-4733-bb30-01e54a4d03cd" />
<img width="1634" height="993" alt="AdobeExpressPhotos_d27f92e902924bb19ce4385971c7c5be_CopyEdited" src="https://github.com/user-attachments/assets/e726e54f-db0b-42df-9dd0-dba777fb983f" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

