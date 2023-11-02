# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

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
```
Developed by:E.kamalesh
RegisterNumber:212222100019
*/

1. Program to design a half adder:

module ex3(a,b,sum,carry);
input a,b;
output sum,carry;
assign sum=a^b;
assign carry=a&b;
endmodule 

2. Program to design a full adder:

module ex31(a,b,cin,sum,carry);
input a,b,cin;
output sum,carry;
assign sum=a^b^cin;
assign carry=(a&b)|((a^b)&cin);
endmodule
```
## Truthtable:

# half adder:
![265629380-f8a33cf4-faec-4a3a-9a45-ba14ae1b5bda](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/788c6da0-84f6-4a85-a355-d59caf032f27)
# full adder:
![265629428-abf97517-ea99-40f1-affd-438e68f6cadb](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/3e87b21d-6068-49db-b858-3c9a6c7f5657)
## RTL realization

# half adder:
![265629708-17b7b349-8cf3-4da8-91e7-6650fd7e733e](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/34c91f50-5076-4be2-b451-94d8a8496ff0)
# full adder:
![265629789-884932e9-6396-4dc5-ad8b-e1d0ef690b61](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/78657342-7edc-40e4-b724-be19fa4681be)
## Output waveform:
# half adder
![265629888-a204ccf6-66f1-43d4-ae24-b980509a1acc](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/84bd8903-c6d4-494d-b132-6bfa5a76d471)
# full adder
![265629963-b5c9748a-da88-428a-9fda-90b04a98d9d0](https://github.com/kamalesh2509/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/120444689/e6fba1ff-7da3-435e-b0d5-cba6e95aa8ad)



### Result:
Thus the half adder and full adder circuit are designed and the truth table for half adder and full adder are verified.

