# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 27/12/25
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>

int main() {
    printf("Integer: %d, Size: %zu bytes\n", 10, sizeof(10));
    printf("Float: %f, Size: %zu bytes\n", 3.14, sizeof(3.14));
    printf("Character: %c, Size: %zu bytes\n", 'A', sizeof('A'));
    printf("String: %s, Size: %zu bytes\n", "Hello C", sizeof("Hello C"));

    return 0;
}
```
# Output:
<img width="1917" height="692" alt="image" src="https://github.com/user-attachments/assets/298b698e-2d5d-4134-917c-5ead6f95e796" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 27/12/25
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>

#define PI 3.14159

int main() {
    const int DAYS = 7;

    printf("Value of PI (Macro): %f\n", PI);
    printf("Value of DAYS (Constant Variable): %d\n", DAYS);

    return 0;
}
```
# Output:
<img width="1917" height="693" alt="image" src="https://github.com/user-attachments/assets/a899f949-94ed-4f40-9983-08618c3b5e1d" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 27/12/25
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>

int main() {
    int age = 20;
    float price = 10.50;
    double distance = 1234.56789;
    char grade = 'A';

    printf("Integer value: %d\n", age);
    printf("Float value: %f\n", price);
    printf("Double value: %lf\n", distance);
    printf("Character value: %c\n", grade);

    return 0;
}
```
# Output:
<img width="1911" height="682" alt="image" src="https://github.com/user-attachments/assets/d5dc5d7e-a7f6-462a-ac27-1f54a005f45b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 27/12/25
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    int a, b;
    scanf("%d %d", &a, &b);
    printf("Arithmetic Operations\n");
    printf("Sum (%d + %d): %d\n", a, b, a + b);
    printf("Difference (%d - %d): %d\n", a, b, a - b);
    printf("Product (%d * %d): %d\n", a, b, a * b);
    printf("Quotient (%d / %d): %d\n", a, b, a / b);
    printf("Remainder (%d %% %d): %d\n", a, b, a % b);
    printf("Bitwise Operations\n");
    printf("AND (%d & %d): %d\n", a, b, a & b);
    printf("OR (%d | %d): %d\n", a, b, a | b);
    printf("XOR (%d ^ %d): %d\n", a, b, a ^ b);
    printf("Left Shift (%d << %d): %d\n", a, b, a << b);
    printf("Right Shift (%d >> %d): %d\n", a, b, a >> b);
    printf("NOT a (~%d): %d\n", a, ~a);
    printf("NOT b (~%d): %d\n", b, ~b);
    return 0;
}
```
# Output:
<img width="1911" height="746" alt="image" src="https://github.com/user-attachments/assets/5d1be732-3fd7-4bf3-96fa-2f3f9106010b" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 27/12/25
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>
int main() {
    char ch;
    scanf("%c", &ch);

    (ch >= '0' && ch <= '9') 
        ? printf("Digit\n") 
        : ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) 
            ? (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' || 
               ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') 
                ? printf("Vowel\n") : printf("Consonant\n") : printf("SpecialSymbol\n");
    return 0;
}
```
# Output:
<img width="1913" height="691" alt="image" src="https://github.com/user-attachments/assets/277f6500-fcb3-4654-9c29-849c6d6529bc" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


