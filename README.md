# Bitwise Operators in C++

##  Overview
This project demonstrates the use of **bitwise operators** in C++.  
Bitwise operators perform operations on the **binary representations** of integers.  
These operators are useful for tasks involving **low-level programming**, such as working with **flags**, **masks**, or performing **efficient calculations**.

---

##  Theory
Bitwise operators work directly on the **bits** of integer data types.  

### Common Bitwise Operators in C++
| Operator | Name                 | Description                                 |
|----------|----------------------|---------------------------------------------|
| `&`      | Bitwise AND          | Sets each bit to 1 if **both** bits are 1   |
| `|`      | Bitwise OR           | Sets each bit to 1 if **at least one** bit is 1 |
| `^`      | Bitwise XOR          | Sets each bit to 1 if **only one** bit is 1 |
| `~`      | Bitwise NOT          | Inverts **all** the bits                    |
| `<<`     | Left Shift           | Shifts bits to the left (**multiplies by 2**) |
| `>>`     | Right Shift          | Shifts bits to the right (**divides by 2**)  |

---

##  Summary of Programs

### 1️⃣ Bitwise Operators Demonstration
This program demonstrates how the **Bitwise AND**, **OR**, **NOT**, **XOR**, **Left Shift**, and **Right Shift** work on two integers.
- **AND (`&`)** → Returns `1` only if both bits are `1`.
- **OR (`|`)** → Returns `1` if at least one bit is `1`.
- **XOR (`^`)** → Returns `1` if the bits are different.
- **NOT (`~`)** → Flips each bit (used for one's complement).
- **Left Shift (`<<`)** → Multiplies a number by `2ⁿ`.
- **Right Shift (`>>`)** → Divides a number by `2ⁿ`.

##  Algorithm
1. **Start** the program.
2. Declare two integer variables `a` and `b` with given values.
3. Calculate:
   - **Bitwise AND**: `bitwise_and = a & b`
   - **Bitwise OR**: `bitwise_or = a | b`
   - **Bitwise NOT**: `bitwise_not = ~a`
   - **Bitwise XOR**: `bitwise_xor = a ^ b`
   - **Left Shift**: `bitwise_leftshift = a << 1`
   - **Right Shift**: `bitwise_rightshift = a >> 1`
4. Display all results on the screen.
5. **End** the program.

---
This is useful to visualize how each bitwise operator affects the **binary representation** of numbers.

---

### 2️⃣ Set and Reset Specific Bits
This program shows how to **set** or **reset** a specific bit in an integer using bitwise operators.
- **To set a bit** → Use **OR (`|`)** with a mask where only the target bit is `1`.
- **Reset (Clear) a bit: Use AND (&) with the complement (~) of a mask where the target bit is `1`.

##  Algorithm

1. **Start** the program.
2. Initialize integer `i = 34` (binary `00100010`) and variables for storing bit positions and results.
3. Prompt the user to **enter the bit position to set**.
4. Create a **bitmask** by shifting `1` left by `bit_to_be_set` positions.
5. **Set the bit** using:  
`set = i | (1 << bit_to_be_set)`
6. Prompt the user to **enter the bit position to reset**.
7. Create a **bitmask** by shifting `1` left by `bit_to_be_reset` positions and applying bitwise NOT (`~`).
8. **Reset the bit** using:  
`reset = i & (~(1 << bit_to_be_reset))`
9. Display the results after setting and resetting.
10. **End** the program.

### Bitwise Operators Demonstration
This program demonstrates the working of:
- **AND (`&`)** → Returns `1` only if both bits are `1`.
- **OR (`|`)** → Returns `1` if at least one bit is `1`.
- **XOR (`^`)** → Returns `1` if the bits are different.
- **NOT (`~`)** → Flips each bit (one's complement).
- **Left Shift (`<<`)** → Multiplies a number by `2ⁿ`.
- **Right Shift (`>>`)** → Divides a number by `2ⁿ`.

##  Conclusion
Bitwise operators are powerful tools in C++ that allow developers to work directly with individual bits of data.  
They provide:
- **Low-level control** over data representation  
- **Performance optimization** in certain algorithms  
- **Efficient memory usage**  
They are especially useful in:
- **Embedded systems** – controlling hardware registers  
- **Graphics programming** – pixel manipulation  
- **Cryptography** – encryption algorithms  
- **Competitive programming** – solving problems with bitmasking  
Mastering bitwise operations enables you to:
- Set, reset, and toggle specific bits  
- Perform quick multiplications/divisions using shift operators  
- Optimize code for speed and efficiency  
