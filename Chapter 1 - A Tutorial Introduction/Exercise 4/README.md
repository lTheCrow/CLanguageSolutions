<h1>Excercise 4</h1>
<h2>Celsius to Fahr Table</h2>
Write a program to print the corresponding Celsius to Fahrenheit table.

Temperature Conversion Program:
```c
#include <stdio.h>

/* print Fahrenheit-Celsius table 
    for fahr = 0, 20, ..., 300; floating-point version */

main()
{
    float fahr, celsius;
    float lower, upper, step;

    lower = 0;          /* lower limit of temperatuire scale */ 
    upper = 300;        /* upper limit */ 
    step = 20;          /* step size */

    fahr = lower;
    while(fahr <= upper){
        celsius = (5.0/9.0) * (fahr-32.0);
        printf("%3.0f %6.1f\n", fahr, celsius);
        fahr = fahr + step;
    }
}
```