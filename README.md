```
Name: Siranjeevi.S
Reg no: 23012822
```
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
## Half Adder 
```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
## Full Adder
```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```

### TRUTH TABLE 

Half Adder Circuit


![ex-3 half table](https://github.com/siranjeevi10/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168132/99b3ba41-2a83-4990-81da-61e092e685bf)


Full Adder Circuit


![ex-3 full table](https://github.com/siranjeevi10/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168132/81901c23-f5a5-40e1-ad5d-4f2453186519)


### RTL

Half Adder Circuit


![ex-3 half RTL](https://github.com/siranjeevi10/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168132/227aef0c-9471-4fba-a484-92e390925ac4)


Full Adder Circuit

![ex-3 full RTL](https://github.com/siranjeevi10/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168132/0d59c8b2-6c5c-4239-8cdb-dabdac9af240)

### Output:

Half Adder Circuit

![ex-3 half diagram](https://github.com/siranjeevi10/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168132/6cb7ab77-2c0c-406d-a7bb-e0457e39ba05)


Full Adder Circuit

![ex-3 full diagram](https://github.com/siranjeevi10/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/152168132/8492bd54-3e49-44b4-8c37-37a7672e7283)

### Result:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.
