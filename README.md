# RPN Calculator Implementation (Data Structures & Algorithms Course Project)

## About HP RPN Calculator

The HP 32SII calculator is a scientific calculator produced by Hewlett-Packard (HP) from 1991 to 2003. It is a successor to the HP 32S and HP 32SII models, and it features a two-line display, an extensive set of scientific and mathematical functions, and a sturdy, high-quality construction.

The calculator has a wide range of features including trigonometric and logarithmic functions, fractions and percentages, statistics, complex numbers, and programming capabilities. It also has a large user memory that can store up to 384 program steps or data registers. The programming language used by the calculator is RPN (Reverse Polish Notation), which requires the user to enter operators aŌer operands. So, no need to convert from Infix to Postfix. I suspect this is because HP used under-powered hardware at the cost of human efforts to convert infix to postfix notations. It made the humans do the hard work. 

The HP 32SII has been praised for its ease of use, reliability, and accuracy, and it remains a popular choice among scientists, engineers, and students. Its sturdy construction, along with its wide range of functions and programmability, make it a versatile tool for a variety of applications.

In recent years, the HP 32SII has become a collector's item, with enthusiasts seeking out original, unopened models and older, well-used models. Its enduring popularity is a testament to its quality and usefulness as a scientific calculator.

## A basic RPN Calculator implementation in C++ 

This RPN calculator program was developed as an attempt to replicate the functionality of a traditional RPN calculator. A basic RPN calculator program that evaluates arithmetic expressions entered by the user in Reverse Polish Notation. It supports basic arithmetic operations such as addition, subtraction, multiplication, and division, as well as more advanced functions such as 
square root, logarithm, sine, cosine, and tangent. 

The program uses two stacks: one for operands and one for operators. The algorithm works by iterating over the input expression one token at a time, and if the token is an operand, it is pushed onto the operand stack. If the token is an operator, the program checks the operator stack to see if there is an operator of higher precedence, and if so, it pops the operator from the operator stack, pops the top two operands from the operand stack, evaluates the expression, and pushes the result back onto the operand stack. This process continues until there are no more operators on the operator stack of higher precedence than the current operator, and then the current operator is pushed onto the operator stack. 

In addition to basic arithmetic operators and functions, the program also supports some additional operations such as taking the factorial of a number and calculating the modulus of two numbers. The program also includes error handling for some operations, such as division by 
zero and taking the square root of a negative number.
