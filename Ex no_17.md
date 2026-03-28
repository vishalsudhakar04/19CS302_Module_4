## DATE: 28-03-2026

## AIM:
To write a C Program to compare two strings without using the built-in `strcmp()` function.

## Algorithm
1. **Start** the program.
2. **Declare** two character arrays (strings) and an integer variable `i` for indexing.
3. **Read** two strings from the user.
4. **Compare** the characters of both strings at each index `i` using a loop:
    * If `str1[i]` is not equal to `str2[i]`, the strings are different.
    * If both reach the null character `\0` at the same time, the strings are identical.
5. **Display** whether the strings are equal or not based on the comparison result.
6. **Stop** the program.

## Program:
```c
#include <stdio.h>
int main() {
    char str1[50], str2[50];
    int i = 0, flag = 0;
    printf("Enter first string: ");
    scanf("%s", str1);
    printf("Enter second string: ");
    scanf("%s", str2);
    while (str1[i] != '\0' || str2[i] != '\0') {
        if (str1[i] != str2[i]) {
            flag = 1;
            break;
        }
        i++;
    }
    if (flag == 0) {
        printf("Strings are equal.\n");
    } else {
        printf("Strings are not equal.\n");
    }
    return 0;
}
```

## Output:
**Case 1:**
```text
Enter first string: Hello
Enter second string: Hello
Strings are equal.
```

**Case 2:**
```text
Enter first string: Apple
Enter second string: Apply
Strings are not equal.
```

## Result:
Thus the program was executed and the output was verified successfully.

---
Would you like me to show you how to make this comparison **case-insensitive** (e.g., treating "Apple" and "apple" as equal)?
