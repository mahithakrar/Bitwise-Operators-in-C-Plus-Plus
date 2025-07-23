# Bitwise-Operators-in-C-Plus-Plus

Overview:
This project demonstrates the use of **bitwise operators** in C++.
Bitwise operators perform operations on the binary representations of integers. 
These operators are useful for tasks involving low-level programming, such as working with flags, masks, or performing efficient calculations.

Theory:
Bitwise operators work directly on the **bits** of integer data types.
Here are the common bitwise operators in C++:
| Operator | Name                 | Description                                 |
|----------|----------------------|---------------------------------------------|
| `&`      | Bitwise AND          | Sets each bit to 1 if both bits are 1       |
| `|`      | Bitwise OR           | Sets each bit to 1 if one of the bits is 1  |
| `^`      | Bitwise XOR          | Sets each bit to 1 if only one bit is 1     |
| `~`      | Bitwise NOT          | Inverts all the bits                        |
| `<<`     | Left Shift           | Shifts bits to the left (multiplies by 2)   |
| `>>`     | Right Shift          | Shifts bits to the right (divides by 2)     |


Summary Of Programs:

1. Bitwise Operators Demonstration
This program demonstrates how the bitwise AND, OR, NOT, XOR, left shift, and right shift work on two integers.
-AND returns 1 only if both bits are 1.
-OR returns 1 if at least one bit is 1.
-XOR returns 1 if the bits are different.
-NOT flips each bit (used for one's complement).
-Left Shift multiplies a number by 2ⁿ.
-Right Shift divides a number by 2ⁿ.
This is useful to visualize how each bitwise operator affects the binary representation of numbers.

2. Set and Reset Specific Bits
This program shows how to set or reset a specific bit in an integer using bitwise operators.
-To set a bit: Use OR (|) with a mask where only the target bit is 1.
-To reset a bit: Use AND (&) with the complement (~) of a mask where the target bit is 1.
For example, if you want to set bit 3, the mask will be 1 << 3. Applying i | mask sets that bit.
To reset bit 4, the mask is again 1 << 4, and i & (~mask) clears that bit.

Conclusion:
Bitwise operators are powerful tools in C++ used for low-level programming, performance optimization, and working directly with binary data. This program helps understand how these operators manipulate individual bits of integer values.
Learning bitwise operations is especially useful in areas like:
1)Embedded systems
2)Graphics programming
3)Cryptography
4)Competitive programming
