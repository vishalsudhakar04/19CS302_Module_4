## DATE: 28-03-2026

## AIM:
To write a C program to find the frequency of a specific character in a given input string.

## Algorithm
1. **Start** the program.
2. **Declare** a character array `str[100]`, a character variable `ch`, and an integer `count` initialized to 0.
3. **Read** the string from the user.
4. **Read** the specific character whose frequency needs to be found.
5. **Traverse** the string using a loop until the null character (`\0`) is reached:
    * If the current character `str[i]` matches the target character `ch`, increment `count`.
6. **Display** the final value of `count`.
7. **Stop** the program.

## Program:
```c
#include <stdio.h>
int main() {
    char str[1000], ch;
    int count = 0, i;
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);
    printf("Enter a character to find its frequency: ");
    scanf("%c", &ch);
    for (i = 0; str[i] != '\0'; ++i) {
        if (ch == str[i]) {
            ++count;
        }
    }
    printf("Frequency of %c = %d\n", ch, count);
    return 0;
}
```

## Output:
```text
Enter a string: programming
Enter a character to find its frequency: r
Frequency of r = 2
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to show you how to find the frequency of **every** character in the string using an array?
