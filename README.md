# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
```
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by:SANJAY S 
RegisterNumber:212222230132
module SANJAY(x,y,s,c);
input x,y;
output s,c;
xor(s,x,y);
and(c,x,y);
endmodule

module full_adder(x, y, z, s, c, x1, x2, x3);
input x,  y,z;
output s ,c, x1, x2, x3;
xor(x1, x, y);
xor(s, x1, z);
and(x2, x, y);
and(x3, x1, z);
or(c, x2, x3);
endmodule
```
*/
Logic symbol & Truthtable
RTL realization

### Output:
### RTL
![image](https://user-images.githubusercontent.com/119091638/234603545-b3093e7d-f671-4426-9f9e-73f600cf8804.png)

![image](https://user-images.githubusercontent.com/119091638/234603715-4a060791-942e-4051-bd8b-d5c1c1b7bcc0.png)

### TIMING DIAGRAM

![image](https://user-images.githubusercontent.com/119091638/234603871-448ce548-09a3-4233-ba0a-a78c0a1c75ea.png)


![image](https://user-images.githubusercontent.com/119091638/234603993-541c0d4b-2ed9-441a-9e8f-40ce25a5401e.png)

### TRUTH TABLE 

![image](https://user-images.githubusercontent.com/119091638/234604152-cc058752-b116-4ddb-a80c-dc1272524b8f.png)

![image](https://user-images.githubusercontent.com/119091638/234604236-e030b500-5838-4384-ad74-5a7b055ba424.png)


### Result:

Therefore,half adder and full adder is verified
