
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
int main() {
 char str[100];
 char *p;
 int vowels = 0, consonants = 0;
 scanf(" %[^\n]", str);
 p = str;
 while (*p != '\0') {
 if ((*p >= 'A' && *p <= 'Z') || (*p >= 'a' && *p <= 'z')) {
 char ch = (*p >= 'A' && *p <= 'Z') ? *p + 32 : *p;
 if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') {
 vowels++;
 } else {
 consonants++;
 }
 }
 p++;
 }
 printf("Vowels: %d\n", vowels);
 printf("Consonants: %d\n", consonants);
 return 0;
}
```

## Output:

![image](https://github.com/user-attachments/assets/f784ea10-37a2-4f06-bd6a-94360113d1db)


## Result:
Thus the program was executed and the output was verified successfully.
