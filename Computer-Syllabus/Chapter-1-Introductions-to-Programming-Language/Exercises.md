# Chapter 1: Programming Exercises

## Exercise 1: Welcome to C Language

- With the help of your teacher, open the IDE installed on your lab computer for writing C programs.
- Write the following program in the editor and save it as "welcome.c".

```c
#include <stdio.h>
#include <conio.h>

void main() 
{
    // A simple C language program
    printf("Welcome to C language");
    getch();
}
```
### Exercise 2: Personal Data of Your Enemy!

Write a program that declares variables of appropriate data types to store personal data about your Enemy. Initialize these variables with the following data:

  Initial letter of their name <br>
  Initial letter of their gender <br>
  Their age <br>
  Their height <br>
```
#include <stdio.h>
#include <conio.h>

void main() 
{
    char initialLetterName = 'I';
    char gender = 'M';
    int age = 20;  //
    float height = 5.2;

    printf("Initial of Name: %c\n", initialLetterName);
    printf("Gender: %c\n", gender);
    printf("Age: %d years\n", age);
    printf("Height: %.1f feet\n", height);

    getch();
}
```
