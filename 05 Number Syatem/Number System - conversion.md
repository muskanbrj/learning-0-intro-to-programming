# Number System Conversions

## Decimal to binary, octal, hexadecimal

Let `N` be the decimal number.  
Let `B` be the base of target number system.  

### Steps:

1. Get remainder when `N` is divided by `B` and write that down
1. Divide `N` by `B` and let `N` be the quotient
1. Repeat the steps 1 & 2 till `N` is not 0
1. Reverse the written number

### Example:  

N = 10  
B = 2
- R = 10 mod 2 = 0, result = 0  
  Q = 10 / 2 = 5, N = 5
- R = 5 mod 2 = 1, result = 01  
  Q = 5 / 2 = 2, N = 2
- R = 2 mod 2 = 0, result = 010  
  Q = 2 / 2 = 1, N = 1
- R = 1 mod 2 = 1, result = 0101  
  Q = 1 / 2 = 0, N = 0  

Result = 1010 (reverse)  
Note: mod means remainder


## Octal to binary

Let `N` be the octal number.  

### Steps:
1. For each digit in `N` convert the digit to 3 digits of binary using Decimal -> Binary
1. Join all the 3 digit binary numbers to form the result
1. Remove leading zeroes.

### Example:  

N = 25  
- Dec 2 = Bin 10, 	3-digit bin = 010
- Dec 5 = Bin 101,	3-digit bin = 101

Result = Bin 010101 = Bin 10101

## Octal to decimal

Let `N` be the octal number  
Let `result` = 0, `place` = 0  

### Steps:
1. For each digit in `N` from right side repeat 2-3
1. Calculate digit x 8<sup> place</sup>, add this to the result
1. place = place + 1

### Example:
N = 25  
- Result = (3 x 8<sup>1</sup>) + (1 x 8<sup>0</sup>) = 24 + 1 = 25

So, Oct 31 = Dec 25


## Octal to hexadecimal

### Steps:
1. Convert Octal to decimal
1. Convert decimal to hexadecimal

### Example:  
N = Oct 32
- Oct 32 = Dec 26
- Dec 26 = Hex 1A

Result = 1A


## Hexadecimal to binary

Let `N` be the hexadecimal number  

### Steps:
1. For each digit in `N` convert the digit to 4 digits of binary using Decimal -> Binary
1. Join all the 4 digit binary numbers to form the result
1. Remove leading zeroes.

### Example:  
N = 2A
- Dec 2 = Bin 10, 	4-digit bin = 0010
- Dec 10 = Bin 1010,	4-digit bin = 1010

Result = Bin 00101010 = Bin 101010

## Hexadecimal to decimal

Let N be the hexadecimal number.  
Let result = 0, place = 0  

### Steps:
- For each digit in N from right side repeat 2-3
- Calculate digit x 16<sup> place</sup>, add this to the result
- place = place + 1

### Example:
N = 2A
- Result = (2 x 16<sup>1</sup>) + (10 x 16<sup>0</sup>) = 32 + 10 = 42

So, Hex 2A = Dec 42

## Hexadecimal to octal

### Steps:
1. Convert hexadecimal to decimal
1. Convert decimal to octal

### Example:
N = Hex 2A
- Hex 2A = Dec 42
- Dec 42 = Oct 52

Result = 52

## Binary to decimal

Let `N` be the binary number  
Let result = 0, place = 0  
### Steps:
1. For each digit in `N` from right side repeat steps 2-3
1. Calculate digit x 2<sup> place</sup>, add this to the result
1. place = place + 1

### Example:
N = 1010  
- Result = (1 x 2<sup>3</sup>) + (0 x 2<sup>2</sup>) + (1 x 2<sup>1</sup>) + (0 x 2<sup>0</sup>) = 8 + 0 + 2 + 0 = 10

So, Bin 1010 = Dec 10

## Binary to octal, hexadecimal

Let `N` be the binary number  
Let `B` be the base of target number system  

### Steps:
- Group 3 digits of binary from right end for octal and 4 digits of binary from right end for hexadecimal.
- If left most group is less than the digits required, add extra leading 0s.
- Convert each group into dec using Bin -> Dec

### Example:
B = 8
N = 10010
Result = 10 010 = 010 010 = 2 2 = 22
So, Bin 10010 = Octal 22

