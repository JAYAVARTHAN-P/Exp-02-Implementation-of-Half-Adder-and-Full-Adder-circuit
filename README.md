## Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit
Implementation-of-Half-Adder-and-Full-Adder-circuit
## AIM:

To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
## Equipments Required:

Hardware – PCs, Cyclone II , USB flasher Software – Quartus prime Theory Adders are digital circuits that carry out addition of numbers.
## Half Adder

Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB
## Full Adder

Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

image
Figure -01 HALF ADDER

image
Figure -02 FULL ADDER
## Procedure :

1 .Connect the supply (+5V) to the circuit. 2 .Switch ON the main switch 3 .If the output is 1, then the led glows.

## Program: 

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.
## Developed by: Jayavarthan P
## RegisterNumber:  212222100015


## HALF ADDER:
```
module exp33(a,b,s,c);
input a,b;
output s,c;
assign s=a^b;
assign c=a&b;
endmodule
```

## FULL ADDER:
```
module ass3(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=a^b^c;
assign carry= ((a&b)|(b&c)|(c&a));
endmodule
```

## Logic symbol & Truthtable RTL realization
## Output:
## RTL
## HALF ADDER:
![264913765-084d609b-1bb0-4f47-82fe-3fb1dda94395](https://github.com/JAYAVARTHAN-P/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121369281/e53f620f-d232-4eb2-b052-3abe24bc9eff)


## FULL ADDER:

![264913797-6ca1e10c-a439-49f7-b7cb-cb7ed7b5e66e](https://github.com/JAYAVARTHAN-P/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121369281/ce17df75-ed7e-441e-845d-7eb8f779b1ad)

## TIMING DIAGRAM:
## HALF ADDER:
![264914200-95eccf36-94f9-4925-ad15-82c9579880aa](https://github.com/JAYAVARTHAN-P/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121369281/d2c3d18b-71ac-43b5-8e08-51630085c329)


## FULL ADDER:
![264913964-863312c7-17df-4b4c-9958-768cbbcf34e6](https://github.com/JAYAVARTHAN-P/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121369281/8371489e-234c-4583-968c-0f4dd6a786ba)


## TRUTH TABLE :
## HALF ADDER:
![264914641-9cd28690-b0b2-4e1f-8f6a-dcf9a657d344](https://github.com/JAYAVARTHAN-P/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121369281/59d964ae-9352-4f28-b466-c0e36a396ccc)



## FULL ADDER:
![264914661-bb1b445a-65fa-4c1f-80fe-aca2993690f6](https://github.com/JAYAVARTHAN-P/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/121369281/9fd101ba-7b30-421a-9f56-4dcfe58f8b5c)

## Result:

Thus the half adder and full adder are studied and the truth table for different logic gates are verified.
