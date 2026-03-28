## DATE: 28-03-2026

## AIM:
To write a C program to perform basic left and right shift operations on a given integer and display the result.

## Algorithm
1. **Start** the program.
2. **Declare** integer variables for the number (`num`) and the number of positions to shift (`pos`).
3. **Read** the integer value and the shift count from the user.
4. **Perform** the Left Shift operation using the `<<` operator (e.g., `num << pos`).
5. **Perform** the Right Shift operation using the `>>` operator (e.g., `num >> pos`).
6. **Display** the results of both operations.
7. **Stop** the program.

## Program:
```c
#include <stdio.h>
int main() {
    int num, pos, left, right;
    printf("Enter an integer: ");
    scanf("%d", &num);
    printf("Enter number of positions to shift: ");
    scanf("%d", &pos);
    left = num << pos;
    right = num >> pos;
    printf("Result after Left Shift (<< %d): %d\n", pos, left);
    printf("Result after Right Shift (>> %d): %d\n", pos, right);
    return 0;
}
```

## Output:
```text
Enter an integer: 10
Enter number of positions to shift: 2
Result after Left Shift (<< 2): 40
Result after Right Shift (>> 2): 2
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to explain how left shifting by $n$ is mathematically equivalent to multiplying by $2^n$?
