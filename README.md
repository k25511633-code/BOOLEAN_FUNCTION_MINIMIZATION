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
```
### Developed by:Kaviya.R

### RegisterNumber:25017570


**RTL realization**
i)
<img width="887" height="436" alt="Screenshot 2025-11-26 183743" src="https://github.com/user-attachments/assets/266c93c9-5773-4ced-90ac-35193ba4120b" />
ii)
<img width="472" height="271" alt="Screenshot 2025-11-26 184522" src="https://github.com/user-attachments/assets/7db9a5c6-8d4d-43f6-be5c-592c420d1dc9" />

**Output:**

**RTL**

**Timing Diagram**
<img width="1919" height="1024" alt="Screenshot 2025-11-26 184033" src="https://github.com/user-attachments/assets/ffdea694-d582-4e2b-b274-e89ef4e30748" />
<img width="1919" height="1018" alt="Screenshot 2025-11-26 184647" src="https://github.com/user-attachments/assets/93bd58f8-9174-40de-b3ea-5c42740855a5" />

**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

