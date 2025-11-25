# HALF_ADDER_SUBTRACTOR

Implementation-of-Half-Adder-and-Half Subtractor-circuit

**AIM:**

To design a half adder and half subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher 

Software – Quartus prime Theory Adders are digital circuits that carry out the addition of numbers.

**Half Adder**

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/bd4a0b2c-cdbc-4184-ab08-81578f121e1f)

Figure -01 HALF ADDER

**Half Subtractor**

The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

Diff = A’B+AB’ =A ⊕ B
Borrow = A’B

 ![image](https://github.com/naavaneetha/HALF_ADDER_SUBTRACTOR/assets/154305477/d76b099c-513f-4e7c-843a-e2fd028a531a)

Figure -02 HALF Subtractor

**Truthtable**
Half adder
![image](https://github.com/user-attachments/assets/bf65359b-fe7f-4c49-9f63-4eed6619f11b)
Full adder
![image](https://github.com/user-attachments/assets/7d7b2e91-8366-4908-a6a6-090659c44506)

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**
 i)HALF ADDER module ha(a,b,sum,carry); input a,b; output sum,carry; assign sum= (a ^ b); assign carry= ( a & b); endmodule ii)HALF SUBTRACTOR module hs(a,b,difference,borrow); input a,b; output difference,borrow; assign difference= (a ^ b); assign borrow= ( ~a & b); endmodule
/* Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by:A.Shruthilaya RegisterNumber:25018192*/

**RTL Schematic**
![image](https://github.com/user-attachments/assets/15dea46e-759f-4141-9e20-3f28b931c574)
![image](https://github.com/user-attachments/assets/4c0c851a-06bd-492b-9ae0-f9aab87b8620)

**Output/TIMING Waveform**
![image](https://github.com/user-attachments/assets/3e6d00c6-6317-4c55-89e0-501c2a4f3205)
![image](https://github.com/user-attachments/assets/6d64beae-f10f-42c4-adf2-56ae5cb3c781)

**Result:**
Thus ,the half adder and half subtractor are studied and the truth table , logic diagram and waveform are verified
