# Mission 5 - Numbers and Data

## Task 5.1 - Convert Numbers by Hand

In this task, I practised converting numbers between decimal, binary and hexadecimal. I used division to convert decimal numbers into binary and place values for the other conversions.

### 1. Convert decimal 13 to binary

I kept dividing 13 by 2 and wrote down the remainders.

13 / 2 = 6, remainder 1
6 / 2 = 3, remainder 0
3 / 2 = 1, remainder 1
1 / 2 = 0, remainder 1
Reading the remainders from bottom to top:

**Answer: 1101**

### 2. Convert decimal 25 to binary

Using the same method:

25 / 2 = 12, remainder 1
12 / 2 = 6, remainder 0
6 / 2 = 3, remainder 0
3 / 2 = 1, remainder 1
1 / 2 = 0, remainder 1
Reading from bottom to top:

**Answer: 11001**

### 3. Convert binary 1010 to decimal

I multiplied each digit by its place value.

1010
= (1 x 8) + (0 x 4) + (1 x 2) + (0 x 1)
= 8 + 0 + 2 + 0

**Answer: 10**

### 4. Convert binary 1101 to decimal

1101
= (1 x 8) + (1 x 4) + (0 x 2) + (1 x 1)
= 8 + 4 + 0 + 1

**Answer: 13**

### 5. Convert hexadecimal A to decimal

In hexadecimal, A represents 10.

A = 10 x 1

**Answer: 10**

### 6. Convert hexadecimal 1F to decimal

In hexadecimal, F represents 15.

1F
= (1 x 16) + (15 x 1)
= 16 + 15

**Answer: 31**

### 7. Convert binary 1111 to hexadecimal

First, I converted the binary number into decimal.

1111
= (1 x 8) + (1 x 4) + (1 x 2) + (1 x 1)
= 8 + 4 + 2 + 1
= 15

In hexadecimal, 15 is written as F.

**Answer: F**

---

## Task 5.2 - Verify Using Python

After doing the conversions by hand, I used Python to check if my answers were correct.
First, I opened Python using this Terminal command:
python3
Then I tried the following expressions.

### 1. Decimal to Binary

Expression: `bin(13)`
Output: `'0b1101'`

Expression: `bin(25)`
Output: `'0b11001'`
Both answers matched my manual calculations. The `bin()` function converts a decimal number into binary. The `0b` at the beginning shows that it is a binary number.

### 2. Binary to Decimal

Expression: `int('1010', 2)`
Output: `10`

Expression: `int('1101', 2)`
Output: `13`
Both answers were correct. The `int()` function converts the given binary number into decimal. The 2 tells Python that the input is in base 2.

### 3. Hexadecimal to Decimal

Expression: `int('A', 16)`
Output: `10`

Expression: `int('1F', 16)`
Output: `31`
These also matched my manual answers. Here, 16 tells Python that the number is hexadecimal.

### 4. Binary to Hexadecimal

Expression: `hex(int('1111', 2))`
Output: `'0xf'`
The answer is F in hexadecimal. First, `int()` converts the binary number into decimal and then `hex()` converts it into hexadecimal. The `0x` shows that it is a hexadecimal number.

### Verification Summary

All my Python results matched the answers I got manually. This helped me check that my conversions were correct.

---

## Task 5.3 - Build a Small Number Converter

For this task, I created a Python file called `number_converter.py`. It asks the user to enter a decimal number and then shows its binary and hexadecimal forms.

### Python functions used

1. `input()` - Takes the number entered by the user.
2. `int()` - Converts the input into an integer.
3. `bin()` - Converts the number into binary.
4. `hex()` - Converts the number into hexadecimal.
5. `print()` - Displays the results.

### Test cases

I tested the program with three different numbers.

| Decimal input | Binary output | Hexadecimal output |
|---|---|---|
| 10 | 1010 | a |
| 25 | 11001 | 19 |
| 42 | 101010 | 2a |

### How the conversion functions work

The `bin()` function converts a number into binary, while `hex()` converts it into hexadecimal. Python adds `0b` before binary values and `0x` before hexadecimal values. In my program, I removed these prefixes from the output.

---

## Task 5.4 - How Is Text Stored?

Computers store text using numbers because they work with numerical data. Character encoding helps give each letter and symbol its own value.

### 1. ASCII codes

- Uppercase A = 65
- Lowercase a = 97

### 2. Why does a computer need an encoding standard?

A computer needs an encoding standard so that letters and symbols can be stored as numbers. It also makes sure that different computers can understand the same text correctly.

### 3. Example of a character outside basic ASCII

The Indian Rupee symbol is not included in basic ASCII. It is supported through Unicode and UTF-8.

### What I understood

I learned how numbers can be converted between decimal, binary and hexadecimal. I also got to practise these conversions myself and check them using Python. Apart from that, I understood how computers use encoding standards to store text and symbols.