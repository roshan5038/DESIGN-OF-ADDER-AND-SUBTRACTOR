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
1.FULL ADDER

![image](https://github.com/user-attachments/assets/c8009776-be29-4bf4-a4e7-2f45ff876961)

2.FULL SUBTRACTER

![image](https://github.com/user-attachments/assets/d1e5747b-9b5e-4641-8138-b9141c7700b7)

**Procedure**

1)Open Quartus2

2)open new file

3)create veri log file and using tools view the logic diagram

4)Then click on netlist viewer and press RTL viewer to view the OUTPUT in graph format

**Program:**

/* Program to design a half subtractor and full subtractor circuit and verify its truth table in quartus using Verilog programming.
```
Developed by: ROSHAN V RegisterNumber:25004228
```
```
1.FULL ADDAR
module ex4(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum = ((a^b)^cin);
assign carry = ((a&b) | (cin & (a ^ b)));
endmodule

2.FULL SUBTRACTED
module ex4(a,b,bin,difference,borrow);
input a,b,bin;
output difference,borrow;
assign difference = ((a^b)^bin);
assign borrow = ((~a&b)|(bin&(~(a^b))));
endmodule
```

**RTL Schematic**
1.FULL ADDER
![image](https://github.com/user-attachments/assets/1ba6fc41-2911-4fad-b5b0-8b022a3db3c2)
2.FULL SUBTRACTER
![image](https://github.com/user-attachments/assets/ec71e06b-88f2-4652-bab2-9571c526689b)

**Output Timing Waveform**
1.FULL ADDER

![image](https://github.com/user-attachments/assets/626a0992-84f9-406a-9538-ab46c05e5917)
2.FULL SUBTRACTER
![image](https://github.com/user-attachments/assets/ef350ac9-433b-49f8-b8ac-b4a64d31606c)


**Result:**

Thus the Full Adder and Full Subtractor circuits are designed and the truth tables is verified using Quartus software.






