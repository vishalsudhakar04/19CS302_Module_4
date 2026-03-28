## DATE: 28-03-2026

## AIM:
To write a C program to convert the given string to lowercase without using any built-in string functions like `strlwr()`.

## Algorithm
1. **Start** the program.
2. **Declare** a character array (string) to store the input.
3. **Read** the string from the user.
4. **Iterate** through the string character by character using a loop until the null character (`\0`) is reached.
5. **Check** if the current character is an uppercase letter (ASCII value between 65 and 90).
6. **Convert** the character to lowercase by adding 32 to its ASCII value if the condition is met.
7. **Display** the modified lowercase string.
8. **Stop** the program.

## Program:
```c
#include <stdio.h>
int main() {
    char str[100];
    int i;
    printf("Enter a string in uppercase: ");
    scanf("%s", str);
    for (i = 0; str[i] != '\0'; i++) {
        if (str[i] >= 'A' && str[i] <= 'Z') {
            str[i] = str[i] + 32;
        }
    }
    printf("String in lowercase: %s\n", str);
    return 0;
}
```

## Output:
```text
Enter a string in uppercase: GEMINI
String in lowercase: gemini
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to show you how to perform the reverse operation—converting a string to **uppercase**?
