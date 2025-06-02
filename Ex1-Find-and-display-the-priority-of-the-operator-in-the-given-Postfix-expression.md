# EX 1 Display operator precedence in the infix expression.

## AIM:
To write a C program to find and display the priority of the operator in the given Postfix expression

## Algorithm
1. Start the program.
2. Define the priority() function to return the priority of operators.
3. Loop through each character in the string.
4. For each operator, call the priority() function to determine its priority.
5. Print the operator and its corresponding priority level.

## Program:
```
Program to find and display the priority of the operator in the given Postfix expression
Developed by: Easwari M
RegisterNumber: 212223240033

#include <stdio.h>
#include<string.h>
int function(char y)
{
    switch(y)
    {
        case '+':
        return 2;
        case '/':
        return 3;
        case '*':
        return 3;
        case '|':
        return 1;
        default:
        return -1;
        
    }
    
}
int main()
{
    char expression[]="100 200 + 2 / 5 * 7|";
    char *x = expression;
    while(*x!=0)
    {
        if(*x=='+' || *x=='/'|| *x=='*'||*x=='|')
        {
            int pr = function(*x);
            printf("%c  ----> ",*x);
            switch(pr)
            {
                case 1:
                printf("Lowest Priority\n");
                break;
                case 2:
                printf("Second Lowest Priority\n");
                break;
                case 3:
                printf("Second Highest Priority\n");
                break;
                case 4:
                printf("Second Highest Priority\n");
            }
        }
        x++;
    }
    return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/4c4fad18-bca9-4aa8-a767-b04dd429506b)

## Result:
Thus the C program to find and display the priority of the operator in the given Postfix expression is implemented successfully
