# EX3 Implementation of Tower of Hanoi
## DATE:
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1.Start the program.
2.Define the priority() function to return the priority of operators.
3.Initialize the string containing operators and operands.
4.Loop through each character in the string.
5.For each operator, call the priority() function to determine its priority.
6.Print the operator and its corresponding priority level. 7.End 

## Program:
```
Program to implement Tower of Hanoi
Developed by: Easwari M
RegisterNumber:  212223240033

#include <stdio.h>

void TOH(int n, char x, char y, char z) {
    if (n == 1) {
        printf("%c to %c\n", x,y);
        return;
    }
    TOH(n - 1, x,z,y);
    printf("%c to %c\n", x,y);
    TOH(n - 1,z,y,x);
}
```

## Output:

![image](https://github.com/user-attachments/assets/86b22a61-6485-4ccf-8b06-38288a3eaf8b)

## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
