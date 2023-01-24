Given an integer, , print the following values for each integer  from  to :

Decimal
Octal
Hexadecimal (capitalized)
Binary
Function Description

Complete the print_formatted function in the editor below.

print_formatted has the following parameters:

int number: the maximum value to print
Prints

The four values must be printed on a single line in the order specified above for each  from  to . Each value should be space-padded to match the width of the binary value of  and the values should be separated by a single space.

Input Format

A single integer denoting .

Constraints

Sample Input

17
Sample Output

    1     1     1     1
    2     2     2    10
    3     3     3    11
    4     4     4   100
    5     5     5   101
    6     6     6   110
    7     7     7   111
    8    10     8  1000
    9    11     9  1001
   10    12     A  1010
   11    13     B  1011
   12    14     C  1100
   13    15     D  1101
   14    16     E  1110
   15    17     F  1111
   16    20    10 10000
   17    21    11 10001
Language
Python 3

More
1234567
def print_formatted(number):
    len_b = len(f'{number:b}')
    for i in range(1,number+1):
        print(f'{i:d}'.rjust(len_b), f'{i:o}'.rjust(len_b), f'{i:X}'.rjust(len_b), f'{i:b}'.rjust(len_b), end='\n') 
if __name__ == '__main__':
    n = int(input())
    print_formatted(n)
Line: 1 Col: 1

Submit Code

Run Code

Upload Code as File

Test against custom input
You have earned 10.00 points!
You are now 40 points away from the 4th star for your python badge.
64%180/220
Python
Congratulations
You solved this challenge. Would you like to challenge your friends?
Share on FacebookShare on TwitterShare on LinkedIn
Next Challenge

Test case 0

Test case 1

Test case 2

Test case 3
Compiler Message
Success
Input (stdin)

Download
2
Expected Output

Download
 1  1  1  1
 2  2  2 10

BlogScoringEnvironmentFAQAbout Us