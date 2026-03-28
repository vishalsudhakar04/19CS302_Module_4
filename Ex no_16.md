## DATE: 28-03-2026

## AIM:
To write a C program to find the minimum between three fraction (floating-point) numbers using the conditional (ternary) operator.

## Algorithm
1. **Start** the program.
2. **Declare** three floating-point variables ($a, b, c$) and one variable for the **minimum** ($min$).
3. **Input** three fractional values from the user.
4. **Use** the nested conditional operator `(condition ? true_val : false_val)` to compare the numbers:
   * $min = (a < b) ? ((a < c) ? a : c) : ((b < c) ? b : c)$
5. **Display** the minimum value found.
6. **Stop** the program.

## Program:
```c
#include <stdio.h>
int main() {
    float a, b, c, min;
    printf("Enter three fraction numbers: ");
    scanf("%f %f %f", &a, &b, &c);
    min = (a < b) ? ((a < c) ? a : c) : ((b < c) ? b : c);
    printf("Minimum value is: %.2f\n", min);
    return 0;
}
```

## Output:
```text
Enter three fraction numbers: 12.5 5.8 9.2
Minimum value is: 5.80
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to show you how to find the **maximum** using the same conditional operator logic?
