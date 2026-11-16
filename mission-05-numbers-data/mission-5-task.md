
# Mission 5 - Numbers and Data

## Task 5.1 - Convert Numbers by Hand

In this task, I practised converting numbers between decimal, binary and hexadecimal. I used the division method for decimal to binary conversions and place values for binary and hexadecimal to decimal conversions.

### 1. Convert decimal 13 to binary
To convert a decimal number into binary, I repeatedly divide the number by 2 and note down the remainder.

13/2 = 6, remainder 1  
6/2 = 3, remainder 0  
3/2 = 1, remainder 1  
1/2 = 0, remainder 1  
Now I read the remainders from bottom to top.

**Answer: 1101**

### 2. Convert decimal 25 to binary
Using the same division method:

25/2 = 12, remainder 1  
12/2 = 6, remainder 0  
6/2 = 3, remainder 0  
3/2 = 1, remainder 1  
1/2 = 0, remainder 1  
Reading the remainders from bottom to top gives:

**Answer: 11001**

### 3. Convert binary 1010 to decimal
For binary to decimal conversion, I multiply each digit by its corresponding power of 2, starting from the right with power 0.

1010
= (1 x 2³) + (0 x 2²) + (1 x 2¹) + (0 x 2⁰)
= (1 x 8) + (0 x 4) + (1 x 2) + (0 x 1)
= 8 + 0 + 2 + 0

**Answer: 10**

### 4. Convert binary 1101 to decimal
I use the same place value method:

1101
= (1 x 2³) + (1 x 2²) + (0 x 2¹) + (1 x 2⁰)
= (1 x 8) + (1 x 4) + (0 x 2) + (1 x 1)
= 8 + 4 + 0 + 1

**Answer: 13**

### 5. Convert hexadecimal A to decimal
Hexadecimal uses base 16. In this system, A represents 10.

A
= 10 x 16⁰
= 10 x 1

**Answer: 10**

### 6. Convert hexadecimal 1F to decimal
In hexadecimal, F represents 15.

1F
= (1 x 16¹) + (15 x 16⁰)
= (1 x 16) + (15 x 1)
= 16 + 15

**Answer: 31**

### 7. Convert binary 1111 to hexadecimal
First, I group the binary digits into groups of four from the right.

1111
The binary value 1111 can be converted into decimal:
= (1 x 8) + (1 x 4) + (1 x 2) + (1 x 1)
= 8 + 4 + 2 + 1
= 15
In hexadecimal, the decimal value 15 is represented by F.

**Answer: F**

---

## Task 5.2 - Verify Using Python

After doing the conversions manually, I used Python's built-in functions to check my answers. I opened the Python interactive environment using Terminal.

Command used:

    python3

I then entered the following expressions one by one.

### 1. Decimal to Binary

Expression:

    bin(13)

Output:

    '0b1101'

Expression:

    bin(25)

Output:

    '0b11001'

Both results match my manual calculations. The `bin()` function converts a decimal integer into binary. The prefix `0b` indicates that the result is in binary.

### 2. Binary to Decimal

Expression:

    int('1010', 2)

Output:

    10

Expression:

    int('1101', 2)

Output:

    13

Both results match my manual calculations. The `int()` function converts a number from the given base into a decimal integer. Here, 2 tells Python that the input is binary.

### 3. Hexadecimal to Decimal

Expression:

    int('A', 16)

Output:

    10

Expression:

    int('1F', 16)

Output:

    31

These results also match my manual calculations. Here, 16 tells Python that the input is hexadecimal.

### 4. Binary to Hexadecimal

Expression:

    hex(int('1111', 2))

Output:

    '0xf'

The result is F in hexadecimal. The `int()` function first converts the binary value into decimal, and `hex()` converts that result into hexadecimal. The prefix `0x` indicates hexadecimal.

### Verification Summary
All the Python results matched the answers I calculated manually. This helped me check whether my conversion steps were correct.

---

## Task 5.3 - Build a Small Number Converter

For this task, I created a Python program called `number_converter.py`.
The program takes a decimal number as input and displays its binary and hexadecimal forms.

### Python functions used

1. `input()` - Takes a number entered by the user.
2. `int()` - Converts the entered value into an integer.
3. `bin()` - Converts the decimal number into binary.
4. `hex()` - Converts the decimal number into hexadecimal.
5. `print()` - Displays the converted results.

### Test cases

I used three positive decimal numbers to check the converter.

| Decimal input | Binary output | Hexadecimal output |
|---|---|---|
| 10 | 1010 | a |
| 25 | 11001 | 19 |
| 42 | 101010 | 2a |

### How the conversion functions work

The `bin()` function takes an integer and returns its binary representation. Similarly, the `hex()` function converts an integer into hexadecimal.

Both functions add a prefix to show the number system being used. For example, `0b` is used for binary and `0x` for hexadecimal.

---

## Task 5.4 - How Is Text Stored?

Computers do not directly understand letters and symbols the way humans do. They store text using character encoding standards, which assign numerical values to characters.

### 1. ASCII codes

The ASCII decimal code for uppercase A is:

65

The ASCII decimal code for lowercase a is:

97

### 2. Why does a computer need an encoding standard?
A computer needs an encoding standard so that every character can be represented using a numerical value that it can store and process. Without a common standard, different systems might interpret the same stored data differently.

### 3. Example of a character outside basic ASCII
The Indian Rupee symbol (₹) is an example of a character that is not part of basic ASCII. It can be represented using Unicode and UTF-8.

### What I understood
Through this task, I understood how computers represent both numbers and text. Different number systems help represent values in different ways, while encoding standards help computers store characters and symbols. I also got to practise the conversions manually and verify them using Python.
