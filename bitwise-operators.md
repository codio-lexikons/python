##Bitwise Operators
Bitwise operator works on bits and perform bit by bit operation. Assume if a = 60; and b = 13; Now in binary format they will be as follows:

```
a = 0011 1100
b = 0000 1101
-----------------
a&b = 0000 1100
a|b = 0011 1101
a^b = 0011 0001
~a  = 1100 0011

```
| Operator |	Description	| Example |
|-|-|-|
|&|	Binary AND Operator copies a bit to the result if it exists in both operands.	|(a & b) will give 12 which is 0000 1100
|**NEED CHARACTER OPTION|	Binary OR Operator copies a bit if it exists in eather operand.	|(a **HELP** b) will give 61 which is 0011 1101
|^|	Binary XOR Operator copies the bit if it is set in one operand but not both.	|(a ^ b) will give 49 which is 0011 0001
|~|	Binary Ones Complement Operator is unary and has the efect of 'flipping' bits.	|(~a ) will give -61 which is 1100 0011 in 2's complement form due to a signed binary number.
|<<|	Binary Left Shift Operator. The left operands value is moved left by the number of bits specified by the right operand.	|a << 2 will give 240 which is 1111 0000
|>>|	Binary Right Shift Operator. The left operands value is moved right by the number of bits specified by the right operand.	|a >> 2 will give 15 which is 0000 1111