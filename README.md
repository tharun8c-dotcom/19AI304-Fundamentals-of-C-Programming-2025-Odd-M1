# 19AI304-Fundamentals-of-C-Programming-2025-Odd-M1
# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 
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
    // Integer literal
    printf("Integer literal: %d\n", 10);
    printf("Size of integer literal: %zu bytes\n\n", sizeof(10));

    // Float literal
    printf("Float literal: %f\n", 3.14f);
    printf("Size of float literal: %zu bytes\n\n", sizeof(3.14f));

    // Character literal
    printf("Character literal: %c\n", 'A');
    printf("Size of character literal: %zu bytes\n\n", sizeof('A'));

    // String literal
    printf("String literal: %s\n", "Hello C");
    printf("Size of string literal: %zu bytes\n\n", sizeof("Hello C"));

    return 0;
}
```

# Output:

<img width="508" height="497" alt="image" src="https://github.com/user-attachments/assets/4e227f8d-a587-4514-8a44-cd922dfd6c38" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 
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

// Step 3: Define a macro constant
#define PI 3.14159

int main() {
    // Step 4: Declare and initialize constant variable
    const int DAYS = 7;

    // Step 5: Print values
    printf("Value of PI (Macro Constant): %.5f\n", PI);
    printf("Value of DAYS (Constant Variable): %d\n", DAYS);

    return 0;
}

```
# Output:

<img width="432" height="217" alt="image" src="https://github.com/user-attachments/assets/a4264477-c9a6-4561-b59b-2d7f1d1a9163" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 
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
    // Step 3: Declare and initialize variables
    int num = 25;
    float price = 19.99f;
    double bigValue = 12345.6789;
    char letter = 'A';

    // Step 4: Display their values
    printf("Integer value: %d\n", num);
    printf("Float value: %.2f\n", price);
    printf("Double value: %.4lf\n", bigValue);
    printf("Character value: %c\n", letter);

    return 0;
}

```
# Output:
<img width="398" height="274" alt="image" src="https://github.com/user-attachments/assets/17fd71ad-be06-4eb9-a092-0b469bd7b106" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 
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

    // Step 4: Input two integers
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    // Step 5: Arithmetic operations
    printf("Arithmetic Operations:\n");
    printf("Sum (a + b) = %d\n", a + b);
    printf("Difference (a - b) = %d\n", a - b);
    printf("Product (a * b) = %d\n", a * b);

    if (b != 0) {
        printf("Quotient (a / b) = %d\n", a / b);
        printf("Remainder (a %% b) = %d\n", a % b);
    } else {
        printf("Quotient (a / b) = Undefined (division by zero)\n");
        printf("Remainder (a %% b) = Undefined (division by zero)\n");
    }

    // Step 6: Bitwise operations
    printf("\nBitwise Operations:\n");
    printf("Bitwise AND (a & b) = %d\n", a & b);
    printf("Bitwise OR (a | b) = %d\n", a | b);
    printf("Bitwise XOR (a ^ b) = %d\n", a ^ b);
    printf("Left Shift (a << 1) = %d\n", a << 1);   // shifting by b is unsafe
    printf("Right Shift (a >> 1) = %d\n", a >> 1);
    printf("Bitwise NOT of a (~a) = %d\n", ~a);
    printf("Bitwise NOT of b (~b) = %d\n", ~b);

    return 0;
}
```
# Output:
<img width="384" height="645" alt="image" src="https://github.com/user-attachments/assets/b15288cd-5738-4cea-9676-4a05d8c90079" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 
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

    // Step 3: Input character
    printf("Enter a character: ");
    scanf("%c", &ch);

    // Step 4–7: Classify using ternary operator
    (ch >= '0' && ch <= '9') ?
        printf("Digit\n") :

    ( (ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z') ) ?
        ( (ch=='a'||ch=='e'||ch=='i'||ch=='o'||ch=='u'||
           ch=='A'||ch=='E'||ch=='I'||ch=='O'||ch=='U') ?
            printf("Vowel\n") :
            printf("Consonant\n") ) :

        printf("Special Symbol\n");

    return 0;
}

```
# Output:

<img width="388" height="237" alt="image" src="https://github.com/user-attachments/assets/542aa305-8c79-4afb-8bcd-5c19423ed8d5" />

<img width="380" height="219" alt="image" src="https://github.com/user-attachments/assets/1ecf18fd-2d73-4429-954c-5c47003120a7" />

<img width="385" height="204" alt="image" src="https://github.com/user-attachments/assets/0c95c5b4-fbfd-44d0-87e3-63accf3a6816" />

<img width="398" height="223" alt="image" src="https://github.com/user-attachments/assets/d74a8715-0a28-489b-8eb3-6b1d9cb0ad88" />





# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


