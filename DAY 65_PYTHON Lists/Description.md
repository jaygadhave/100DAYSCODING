Consider a list (list = []). You can perform the following commands:

insert i e: Insert integer  at position .
print: Print the list.
remove e: Delete the first occurrence of integer .
append e: Insert integer  at the end of the list.
sort: Sort the list.
pop: Pop the last element from the list.
reverse: Reverse the list.
Initialize your list and read in the value of  followed by  lines of commands where each command will be of the  types listed above. Iterate through each command in order and perform the corresponding operation on your list.

Example





: Append  to the list, .
: Append  to the list, .
: Insert  at index , .
: Print the array.
Output:
[1, 3, 2]
Input Format

The first line contains an integer, , denoting the number of commands.
Each line  of the  subsequent lines contains one of the commands described above.

Constraints

The elements added to the list must be integers.
Output Format

For each command of type print, print the list on a new line.

Sample Input 0

12
insert 0 5
insert 1 10
insert 0 6
print
remove 6
append 9
append 1
sort
print
pop
reverse
print
Sample Output 0

[6, 5, 10]
[1, 5, 9, 10]
[9, 5, 1]
Language
Pypy 3

More
1234567891011121314151617181920
if __name__ == '__main__':
    N = int(input())
    list=[]
    p=0
    for item in range(N):
       sotre=input().split()
       if sotre[0]=="insert":
        list.insert(int(sotre[1]),int(sotre[2]))
       elif sotre[0]=="remove":
        list.remove(int(sotre[1]))
       elif sotre[0]=="append":
        list.append(int(sotre[1]))
       elif sotre[0]=="sort":
        list.sort()
       elif sotre[0]=="pop":
        list.pop()
       elif sotre[0]=="reverse" :
        list.reverse()  
       elif sotre[0]=="print":
        print(list) 
Line: 20 Col: 21

Submit Code

Run Code

Upload Code as File

Test against custom input
Python
You have earned 10.00 points!
You are now 10 points away from the 3rd star for your python badge.
75%100/110
Congratulations
You solved this challenge. Would you like to challenge your friends?Share on FacebookShare on TwitterShare on LinkedIn
Next Challenge

Test case 0

Test case 1
Compiler Message
Success
Input (stdin)

Download
12
insert 0 5
insert 1 10
insert 0 6
print
remove 6
append 9
append 1
sort
print
pop
reverse
print
Expected Output

Download
[6, 5, 10]
[1, 5, 9, 10]
[9, 5, 1]
Blog