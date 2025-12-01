
# EX 24 Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
## DATE: 
## AIM:
To Create a structure program to read(empno,dept and basic pay) and store the data of 3 employees and calculate their Gross Salary(da =10% and HRA=30% from BP).

## Algorithm
1. Start.
2. Define a variables.
3. Create a structure program to read(empno,dept and basic pay) and store the data of 3
employees and calculate their Gross Salary(da =10% and HRA=30% from BP).
4. Read the value using scanf.
5. Ask the user to make an input.
6. Print out the answer.
7. End.

## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>

struct emp
{
    int empno;
    char dept[50];
    float bp;
};

int main()
{
    struct emp e[3];
    int i;

    for (i = 0; i < 3; i++)
        scanf("%d %s %f", &e[i].empno, e[i].dept, &e[i].bp);

    printf("Details of the Employee:\n");

    for (i = 0; i < 3; i++)
    {
        float da = e[i].bp * 0.10;
        float hra = e[i].bp * 0.30;
        float gross = e[i].bp + da + hra;

        printf("%d %s %.0f %.0f %.0f %.2f\n",
               e[i].empno, e[i].dept,
               e[i].bp, da, hra, gross);
    }

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/909f7e04-30a1-4e03-b32e-fdc230702edc)


## Result:
Thus the program was executed and the output was verified successfully.
