# Chapter 2: Programming Exercises

### Exercise 1:
The criteria for the calculation of wages in a company is given below:

- Basic Salary = Pay Rate Per Hour × Working Hours Of Employee
- Overtime Salary = Overtime Pay Rate × Overtime Hours Of Employee
- Total Salary = Basic Salary + Overtime Salary

Write a program that should take the working hours and overtime hours of the employee as input. The program should calculate and display the total salary of the employee.

```c
#include <stdio.h>

int main() {
    float payRate, overtimePayRate, workingHours, overtimeHours, basicSalary, overtimeSalary, totalSalary;

    // Input
    printf("Enter Pay Rate Per Hour: ");
    scanf("%f", &payRate);
    printf("Enter Working Hours of Employee: ");
    scanf("%f", &workingHours);
    printf("Enter Overtime Pay Rate: ");
    scanf("%f", &overtimePayRate);
    printf("Enter Overtime Hours of Employee: ");
    scanf("%f", &overtimeHours);

    // Calculations
    basicSalary = payRate * workingHours;
    overtimeSalary = overtimePayRate * overtimeHours;
    totalSalary = basicSalary + overtimeSalary;

    // Output
    printf("Total Salary of Employee: %.2f\n", totalSalary);

    return 0;
}
```
### Exercise 2:

Write a program that takes Celsius temperature as input, converts the temperature into Fahrenheit, and shows the output. The formula for conversion is:
F = (9/5) * C + 32
```
#include <stdio.h>

int main() {
    float celsius, fahrenheit;

    // Input
    printf("Enter Temperature in Celsius: ");
    scanf("%f", &celsius);

    // Conversion
    fahrenheit = (9.0/5.0) * celsius + 32;

    // Output
    printf("Temperature in Fahrenheit: %.2f\n", fahrenheit);

    return 0;
}
```
### Exercise 3:

Write a program that displays the following output using a single printf statement:
```
*
**
***
****
*****
```
```
#include <stdio.h>

int main() {
    printf("*\n**\n***\n****\n*****\n");
    return 0;
}
```
### Exercise 4:

Write a program that displays the following output using a single printf statement:
```
I am a Boy
I am is QuickSilver
I am is proud of Being QuickSilver
```
```
#include <stdio.h>

int main() {
    printf("I am a Boy\nI am is QuickSilver\nI am is proud Being QuickSilver\n");
    return 0;
}
```
### Exercise 5:

A clothing brand offers a 15% discount on each item. A lady buys 5 shirts from this brand. Write a program that calculates the total price after discount and the amount of discount availed by the lady. The original prices of the shirts are:

  Shirt1 = 423
  Shirt2 = 320
  Shirt3 = 270
  Shirt4 = 680
  Shirt5 = 520
```
#include <stdio.h>

int main() {
    float shirt1 = 423, shirt2 = 320, shirt3 = 270, shirt4 = 680, shirt5 = 520;
    float discount = 0.15, totalOriginalPrice, totalDiscount, totalPriceAfterDiscount;

    // Calculation
    totalOriginalPrice = shirt1 + shirt2 + shirt3 + shirt4 + shirt5;
    totalDiscount = totalOriginalPrice * discount;
    totalPriceAfterDiscount = totalOriginalPrice - totalDiscount;

    // Output
    printf("Total Original Price: %.2f\n", totalOriginalPrice);
    printf("Total Discount: %.2f\n", totalDiscount);
    printf("Total Price After Discount: %.2f\n", totalPriceAfterDiscount);

    return 0;
}
```
### Exercise 6:

Write a program that swaps the values of two integer variables without the help of any third variable.
```
#include <stdio.h>

int main() {
    int a, b;

    // Input
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    // Swap without third variable
    a = a + b;
    b = a - b;
    a = a - b;

    // Output
    printf("After swapping: a = %d, b = %d\n", a, b);

    return 0;
}
```
### Exercise 7:

Write a program that takes a 5-digit number as input, calculates, and displays the sum of the first and last digits of the number.
```
#include <stdio.h>

int main() {
    int num, firstDigit, lastDigit, sum;

    // Input
    printf("Enter a 5-digit number: ");
    scanf("%d", &num);

    // Calculation
    lastDigit = num % 10;
    firstDigit = num / 10000;
    sum = firstDigit + lastDigit;

    // Output
    printf("Sum of first and last digit: %d\n", sum);

    return 0;
}
```
### Exercise 8:

Write a program that takes the monthly income and monthly expenses (e.g., electricity bill, gas bill, food expense) of the user. The program should calculate the following:

  Total monthly expenses
  Total yearly expenses
  Monthly savings
  Yearly savings
  Average savings per month
  Average expenses per month
```
#include <stdio.h>

int main() {
    float income, electricity, gas, food, totalExpenses, totalYearlyExpenses, monthlySavings, yearlySavings, avgMonthlySavings, avgMonthlyExpenses;

    // Input
    printf("Enter monthly income: ");
    scanf("%f", &income);
    printf("Enter electricity bill: ");
    scanf("%f", &electricity);
    printf("Enter gas bill: ");
    scanf("%f", &gas);
    printf("Enter food expense: ");
    scanf("%f", &food);

    // Calculations
    totalExpenses = electricity + gas + food;
    totalYearlyExpenses = totalExpenses * 12;
    monthlySavings = income - totalExpenses;
    yearlySavings = monthlySavings * 12;
    avgMonthlySavings = monthlySavings;
    avgMonthlyExpenses = totalExpenses;

    // Output
    printf("Total Monthly Expenses: %.2f\n", totalExpenses);
    printf("Total Yearly Expenses: %.2f\n", totalYearlyExpenses);
    printf("Monthly Savings: %.2f\n", monthlySavings);
    printf("Yearly Savings: %.2f\n", yearlySavings);
    printf("Average Savings per Month: %.2f\n", avgMonthlySavings);
    printf("Average Expenses per Month: %.2f\n", avgMonthlyExpenses);

    return 0;
}
```
### Exercise 9:

Write a program that takes a character and the number of steps as input from the user. The program should then "jump" the number of steps from that character.
```
#include <stdio.h>

int main() {
    char ch;
    int steps;

    // Input
    printf("Enter a character: ");
    scanf(" %c", &ch);
    printf("Enter number of steps: ");
    scanf("%d", &steps);

    // Calculation
    char newChar = ch + steps;

    // Output
    printf("New character: %c\n", newChar);

    return 0;
}
```
### Exercise 10:

Write a program that takes the radius of a circle as input. The program should calculate and display the area of the circle.
```
#include <stdio.h>
#define PI 3.14159

int main() {
    float radius, area;

    // Input
    printf("Enter radius of the circle: ");
    scanf("%f", &radius);

    // Calculation
    area = PI * radius * radius;

    // Output
    printf("Area of the circle: %.2f\n", area);

    return 0;
}
```
