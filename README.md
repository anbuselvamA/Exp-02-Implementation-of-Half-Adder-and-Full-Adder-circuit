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
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
```
Developed by: Anbuselvam A
RegisterNumber:  212222240009
Half adder program:

module fulladd (a,b,sum,carry);

input a,b;

output sum,carry;

assign sum = (a^b);

assign carry = (a&b);

endmodule

Full adder program:

module fulladd (a,b,c,sum,carry);

input a,b,c;

output sum,carry;

assign sum = (a^b^c);

assign carry = ((a&b)|(a^b)&c);

endmodule
```
*/
Logic symbol & Truthtable
RTL realization

### Output:
Half adder:
![01](https://user-images.githubusercontent.com/119559871/233826948-5f3437a6-33c4-4bdd-9f53-a3a682acc952.png)

Full adder:
![02](https://user-images.githubusercontent.com/119559871/233826986-4e091667-de85-4a1c-be7a-8b21c18baafe.png)

### RTL
Half adder:
![03](https://user-images.githubusercontent.com/119559871/233827026-271cc363-68bc-4e8e-83b1-0a0483211a83.png)


Full adder:
![04](https://user-images.githubusercontent.com/119559871/233827061-f861749f-f1b1-457a-96c9-bee662acd24d.png)


### TIMING DIAGRAM
Half adder :
![05](https://user-images.githubusercontent.com/119559871/233827130-059d626d-fd08-4c17-a223-c03b2c053170.png)



Full adder:
![06](https://user-images.githubusercontent.com/119559871/233827148-660365f5-0b30-4121-8fe0-a874560eb638.png)


### TRUTH TABLE 
Half adder:
![07](https://user-images.githubusercontent.com/119559871/233827178-e18a8886-f287-43de-856b-20e89399340c.png)

Full adder :
![08](https://user-images.githubusercontent.com/119559871/233827208-de118a20-bb97-4f79-a3a0-b3b47d1f6c74.png)


### Result:
Thus the Implementation of Half Adder and Full Adder circuit are studied and the truth table for different logic gates are verified.


