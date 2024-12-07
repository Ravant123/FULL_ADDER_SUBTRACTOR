# FULL_ADDER_SUBTRACTOR

Implementation-of-Full-Adder-and-Full-subtractor-circuit

**AIM:**

To design a Full Adder and Full Subtractor circuit and verify its truth table in Quartus using Verilog programming.

**Equipments Required:**

Hardware – PCs, Cyclone II , USB flasher

Software – Quartus prime

**Full Adder and Full Subtractor**

**Full Adder**

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin 

Carry = AB + ACin + BCin

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/0f30ba51-5ffb-4198-845f-18e054f675e7)

**Figure -1 FULL ADDER**

**Full Subtractor**

A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow.

![image](https://github.com/naavaneetha/FULL_ADDER_SUBTRACTOR/assets/154305477/02b24f51-ab51-4304-9ad6-7b81ffc1ead5)

Diff = A ⊕ B ⊕ Bin 

Borrow out = A'Bin + A'B + BBin

**Truthtable**

FULL ADDER

![1](https://github.com/user-attachments/assets/1d73a6ab-ab7d-4be4-ba36-f274532a2dc9)

FULL SUBTRACTOR

![2](https://github.com/user-attachments/assets/5503014a-333b-45cc-8621-a796178dfc46)

**Procedure**

Write the detailed procedure here

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.

Full adder
    
    module fa(a,b,cin,sum,carry);
    input a,b,cin;
    output sum,carry;
    assign sum=( (a ^ b)^cin);
    assign carry= ( (a & b)| ( cin &(a ^ b )));
    endmodule

Full subtractor

    module fs(a,b,bin,difference,borrow);
    input a,b,bin;
    output difference,borrow;
    assign difference= ( (a ^ b)^bin);
    assign borrow= ( ( ~a & b)| ( bin & (~(a ^ b ))));
    endmodule
  



Developed by:S.Ravant Vignesh
RegisterNumber:24900151
*/

**RTL Schematic**
![3](https://github.com/user-attachments/assets/cdae53e4-8e5d-4e18-a7d3-4961b8b17421)

![4](https://github.com/user-attachments/assets/e6d3d565-68e8-4d9b-b205-5d6975b96855)


**Output Timing Waveform**
![5](https://github.com/user-attachments/assets/32472f75-cefa-40be-8dbc-1079f5fb24ad)

![6](https://github.com/user-attachments/assets/4a634102-bafa-42a0-a169-51f91158d7db)

**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.



