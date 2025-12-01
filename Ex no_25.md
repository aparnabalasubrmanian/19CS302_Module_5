
# EX 25 C program to check whether a given character is a vowel or consonant using pointer
## DATE: 11.7.25
## AIM:
To write a C program to check whether a given character is a vowel or consonant using pointer

## Algorithm
1. Start.
2. Declare a variable value of type char.
3. Prompt the user to enter a value.
4. Read the value using scanf.
5. Find vowel and consonants
6. End.

## Program:
```
/*
Developed by: Aparna RB
RegisterNumber:  212222220005
*/
#include <stdio.h>

int main()
{
    char s[100];
    int vowels = 0, consonants = 0;
    char *p;

    fgets(s, sizeof(s), stdin);
    p = s;

    while (*p)
    {
        if (*p >= 'A' && *p <= 'Z')
            *p = *p + 32;

        if (*p >= 'a' && *p <= 'z')
        {
            if (*p == 'a' || *p == 'e' || *p == 'i' || *p == 'o' || *p == 'u')
                vowels++;
            else
                consonants++;
        }
        p++;
    }

    printf("Vowels: %d\nConsonants: %d", vowels, consonants);

    return 0;
}

```

## Output:

![image](https://github.com/user-attachments/assets/f784ea10-37a2-4f06-bd6a-94360113d1db)


## Result:
Thus the program was executed and the output was verified successfully.
