# Day 1: Data Types

### Problem Link <a id="problem"></a>

* [x] [**HackerRank Problem Link**](https://www.hackerrank.com/challenges/30-data-types/problem)\*\*\*\*

### Solution

* [x] **In C Language**

{% code title="Data\_Types.c" %}
```c
#include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>

int main() {
    int i = 4;
    double d = 4.0;
    char s[] = "HackerRank ";

    
    // Declare second integer, double, and String variables.
    
    int i2;
    double d2;
    char s2[100];
    
    // Read and save an integer, double, and String to your variables.
    
    scanf("%d", &i2);
    scanf("%lf", &d2);
    
    // Print the sum of both integer variables on a new line.
    
    scanf("%*[\n] %[^\n]", s2);
    
    // Print the sum of the double variables on a new line.
    
    printf("%d\n", i + i2);
    
    // Concatenate and print the String variables on a new line
   
    printf("%.01lf\n", d + d2);
   
    // The 's' variable above should be printed first.
    
    printf("%s%s", s, s2);

    return 0;
}
```
{% endcode %}

