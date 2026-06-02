# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M4
# IAPR-4- Module 4 - FoC
## 7. Implementation of Functions.
## 8. Implementation of passing parameters.
# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
    int num = 44;
    int shift = 3;
    int result;
    result = num << shift;
    printf("Number before left shift: %d\n", num);
    printf("Number after left shift by %d positions: %d\n", shift, result);
    return 0;
}

```
## OUTPUT
<img width="1046" height="625" alt="M41" src="https://github.com/user-attachments/assets/639d28fe-b64b-4499-9936-237b08845f1a" />


## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
    int a, b;
    scanf("%d %d", &a, &b);
    if(a == b)
        printf("Both numbers are equal.\n");
    if(a != b)
        printf("Both numbers are not equal.\n");
    return 0;
}

```

## OUTPUT
<img width="1049" height="616" alt="M42" src="https://github.com/user-attachments/assets/f9f4d39a-7c32-4172-904c-b8746cd4f34b" />


## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <ctype.h>
int main() {
    char str[100];
    int i;
    scanf("%[^\n]", str);
    for(i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }
    printf("String in lowercase: %s\n", str);
    return 0;
}

```

## OUTPUT
<img width="1048" height="616" alt="M43" src="https://github.com/user-attachments/assets/094f7093-5c2f-4e5d-92d3-8f7f07bea19a" />



## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>
int main() {
    char str[200];
    int i = 0, count = 1;
    scanf("%[^\n]", str);
    do {
        if(str[i] == ' ' || str[i] == '\t')
            count++;
        i++;
    } while(str[i] != '\0');
    printf("Total number of words: %d\n", count);
    return 0;
}

```

## OUTPUT

<img width="1045" height="617" alt="M44" src="https://github.com/user-attachments/assets/b5405d59-6e07-4b45-a313-3b88a0359e64" />




## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
<br>
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable,flag and initialize it to 0, and i for indexing. 
<br>
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
<br>
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
<br>
Step 5: Start comparing characters of both strings from index i = 0.
<br>
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
<br>
•	If c1[i] is not equal to c2[i], set flag = 1.
<br>
•	Increment i by 1.
<br>
Step 7: After the loop, check the value of flag:
<br>
•	If flag == 0, print "strings are same".
<br>
•	Otherwise, print "strings are not same".
<br>
Step 8: End the program.
<br>

## PROGRAM
```
#include <stdio.h>
int main() {
    char str1[100], str2[100];
    int i = 0, flag = 0;
    scanf("%s", str1);
    scanf("%s", str2);
    while(str1[i] != '\0' || str2[i] != '\0') {
        if(str1[i] != str2[i]) {
            flag = 1;
            break;
        }
        i++;
    }
    if(flag == 0)
        printf("Both strings are equal.\n");
    else
        printf("Strings are not equal.\n");
    return 0;
}

```


## OUTPUT
<img width="1276" height="754" alt="M45" src="https://github.com/user-attachments/assets/cf93fbb0-0b3d-4f78-a1c0-0233ea4c54d9" />


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.
