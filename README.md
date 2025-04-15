# CODETECH-Task1
Name - Soundarya Badiger
Company - CODEYECH IT SOLUTIONS
ID - CT04WM61
Domain -VLSI
Duration -March 18th,2025 to April 18th,2025
Mentor - Vaishali

Here's an overview of the alu_32bit_case Verilog module:


---

Module Name: alu_32bit_case

Purpose:

This module implements a 32-bit Arithmetic Logic Unit (ALU) using a case statement, performing different operations based on a 3-bit control input f.


---

Inputs:

a [31:0]: First 32-bit input operand

b [31:0]: Second 32-bit input operand

f [2:0]: 3-bit function selector (control signal)


Output:

y [31:0]: 32-bit result of the selected ALU operation



---

Functionality:

Based on the value of f, the module performs the following:

The alu_32bit_case module performs different operations based on the 3-bit control input f. When f is 3'b000, the ALU performs a bitwise AND operation between inputs a and b. If f is 3'b001, it carries out a bitwise OR. For f equal to 3'b010, the ALU executes a bitwise NOR by taking the complement of the OR operation between a and b. When f is set to 3'b011, the module adds the two inputs, while f = 3'b100 results in subtraction of b from a. Lastly, when f is 3'b101, the module performs multiplication of a and b. If the control signal f has any other value, the output y is set to an undefined state (32'bx).

---

Use Case:

This ALU is typically used in processors or digital systems that require a small set of arithmetic and logic operations. The control signal (f) determines which operation the ALU will execute on the given operands.


---
