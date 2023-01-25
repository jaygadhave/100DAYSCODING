Polar coordinates are an alternative way of representing Cartesian coordinates or Complex Numbers.

A complex number Capture.PNG
is completely determined by its real part  and imaginary part .
Here,  is the imaginary unit.
A polar coordinate ()Capture.PNG

is completely determined by modulus  and phase angle .

If we convert complex number  to its polar coordinate, we find:
: Distance from  to origin, i.e., 
: Counter clockwise angle measured from the positive -axis to the line segment that joins  to the origin.

Python's cmath module provides access to the mathematical functions for complex numbers.


This tool returns the phase of complex number  (also known as the argument of ).

>>> phase(complex(-1.0, 0.0))
3.1415926535897931

This tool returns the modulus (absolute value) of complex number .

>>> abs(complex(-1.0, 0.0))
1.0
Task
You are given a complex . Your task is to convert it to polar coordinates.

Input Format

A single line containing the complex number . Note: complex() function can be used in python to convert the input as a complex number.

Constraints

Given number is a valid complex number

Output Format

Output two lines:
The first line should contain the value of .
The second line should contain the value of .

Sample Input

  1+2j
Sample Output

 2.23606797749979 
 1.1071487177940904
Note: The output should be correct up to 3 decimal places.

Language
Python 3

More
1234
import cmath
num=complex(input())
print(abs(complex(num)))
print(cmath.phase(complex(num)))
Line: 4 Col: 33

Submit Code

Run Code

Upload Code as File

Test against custom input
Python
You have earned 10.00 points!
You are now 30 points away from the 4th star for your python badge.
73%190/220
Congratulations
You solved this challenge. Would you like to challenge your friends?Share on FacebookShare on TwitterShare on LinkedIn
Next Challenge

Test case 0

Test case 1

Test case 2

Test case 3

Test case 4

Test case 5
Compiler Message
Success
Input (stdin)

Download
1+2j
Expected Output

Download
2.23606797749979
1.1071487177940904
Blog