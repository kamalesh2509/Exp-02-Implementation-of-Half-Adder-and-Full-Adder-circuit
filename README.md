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

### Program:

```### HALF ADDER PROGRAM
module HALFADDER(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b);
endmodule
### FULL ADDER PROGRAM
module FULLADDER(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule
```

```
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
Developed by: E.kamalesh
RegisterNumber:  212222100019
```



### Output:
### RTL
![232856532-b831cbc1-33f3-4d65-a125-d5e5f6df8f29](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/25f4bff6-15c8-4c0e-9831-c2d1cb1808b8)

![232956381-d1cb7dc8-7c60-47e0-ac44-3acd93e24137](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/cefa792c-ac34-4d5e-858e-9df6e066df35)


### TIMING DIAGRAM
![232856729-3b9025a8-342a-44d6-ab78-38d14782a5f9](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/473f6a0f-a919-49d7-94d7-25f474d2488a)

![232956501-e9b9cca6-e516-4338-a103-e8b8906d73ae](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/8c96e62a-c6be-4bd1-9e6f-7449ca42fc18)


### TRUTH TABLE
![232856995-e7c3449b-1115-4cc8-833f-8e31db7684c2](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/ac609db8-f757-4138-95ca-832761d87dab)

![232856995-e7c3449b-1115-4cc8-833f-8e31db7684c2](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/f9b5db62-2217-4574-b368-4f3dd986c717)


### Result:

Thus, a half adder and full adder circuit is designed to verify its truth table in Quartus using Verilog programming.
