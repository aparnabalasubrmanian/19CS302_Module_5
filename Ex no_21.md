
# EX 21 C program to calculate the area of a triangle using pointer.
## DATE: 
## AIM:
To write a C program to calculate the area of a triangle using pointer.

## Algorithm
1. Start.
2. Declare three variable value of type float.
3. Prompt the user to enter values.
4. Read the values using scanf.
5. Find the area of triangle using formula
6. End  

## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>
int main() {
 float base, height, area;
 float *pBase = &base, *pHeight = &height;
 scanf("%f", pBase);
 scanf("%f", pHeight);
 area = 0.5 * (*pBase) * (*pHeight);
 printf("%.2f\n", area);
}

```

## Output:

![Screenshot 2025-04-30 154838](https://github.com/user-attachments/assets/61464af2-29b1-49a6-be06-80db54e3ef59)


## Result:
Thus the program was executed and the output was verified successfully.
