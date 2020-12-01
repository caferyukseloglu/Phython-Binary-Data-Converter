# Binary Data Converter

The purpose of this assignment is to become more familiar with bit-level
representations of integers and floating-point numbers. 
* a hexadecimal number and
* the data type to be converted, 

as input and converts the number according to the predefined format and gives
the converted data as output.

The data type can be any of the following:
* signed integer (S)
* unsigned integer (U)
* floating point number (F)

The size of the input can be 1, 2, 3 and 4 bytes, if input is other than these
sizes then an error message will be given.

* If the selected data type is signed integer, your program will convert the
number using 2’s complement representation.
* If the selected data type is unsigned integer, number will be converted using
unsigned integer representation.
* If the selected data type is floating point number, you will use IEEE-like
format. The number of exponent bits according to given data size will be like
the following:
``` if 1 byte (i.e., 8 bits), 4 bits will be used for exponent part
if 2 bytes (i.e., 16 bits), 6 bits will be used for exponent part

if 3 bytes (i.e., 24 bits), 8 bits will be used for exponent part

if 4 bytes (i.e., 32 bits), 10 bits will be used for exponent part

For each given data size 1 bit will be used for sign and remaining bits will be used for fraction.

While calculating the mantissa to get the floating-point value, you will only use the first 13 bits of the fraction part (If the data size is 3 or 4 bytes).
You will use “round to even” method for rounding fraction bits to 13 bits.
```

## Details

Details about the program are listed below:
* At the beginning of the execution, your program will prompt for the input.
If the input has odd number of characters complete it to even by adding
0 to the MSB.
```
▪ If the number entered is A57, it will be stored as 0A57 and
its size is 2 bytes.
▪ If the number is 12345, it will be stored as 012345, and its
size is 3 bytes.
▪ If the input is 123456789, then an error message is given.
(bigger than 4 byte)
▪ Any inappropriate input results an error message. (Only
digits and characters from A to F will be accepted as an
input)

Floating point numbers may be NaN, +0, -0 or infinity. In these cases, the
output will be:
• NaN
• ∞
• -∞
• 0
• -0

For the output, the floating-point numbers will have precision of maximum
5 digits after the decimal point.
• You cannot use library functions for the binary to decimal conversions.
```

## License
[MIT](https://choosealicense.com/licenses/mit/)
