[Back to Portfolio](./)

Columnar Cipher Coder
===============

-   **Class:** CSCI 452
-   **Grade:** 90
-   **Language(s):** C++
-   **Source Code Repository:** [features/mastering-markdown](https://guides.github.com/features/mastering-markdown/)  
    (Please [email me](mailto:example@csustudent.net?subject=GitHub%20Access) to request access.)

## Project description

Columnar Cipher Coder is a set of C++ files that can be compiled as standalone programs or as part of a project. There are two files: an encoder and decoder.
The encoder uses columnar disposition to take a 36 character message and enter it into a character array, 
and then prints the array into a new 36 character message according to the column order provided by 
the end user. The decoder will take the encrypted message and place it into a character array and
display the plaintext message by printing the columns in the order provided by the user, which
usually is the "key".

## How to compile the project:

Windows CMD/Linux Terminal/MacOS Bash
```
cd ./project
g++ -Wextra -o [filename] [filename].cpp
```

## How to run the project:
Windows 64x
```
find the project in project folder and choose encoder.exe for the encoder
and decoder.exe for the decoder
```

## UI Design

The Columnar Cipher Encoder works by recieving a 36 character message and encrypting it by inserting it into 6 columns 
and displaying the information in each column top-down, and the order of the columns is determined by the user.
The Columnar Cipher Decoder takes the 36 character encrypted message and breaks it into 6 columns, and displays the columns top-down according to the user. 

For encryption, the user will enter a 36 character message exactly, and provide a key using 6 numbers from 0 to 5(Ex. 012345) in whatever desired order to arrage the columns and will print the encrypted message (see Fig 1). This will become the "key". The user can then enter the encrypted message into the decoder and enter the key or manually generate one from a keyword and enter it when prompted, which will generate the plaintext message (see Fig 1). 

![screenshot](images/columnar_cipher_ss.png)  
Fig 1. encoder and decoder in action, as well as a test of 'ASDFGH' in correct order 
with a provided key for expected results.

## 3. Additional Considerations

The program is meant to handle exactly 36 characters and it is not advised to use spaces or special characters. It is not case-sensitive
and will receive input whether capitalized or not. For keys, the user will enter a 6 digit code with each digit being unique and non-repeated
from 0 and 5 (Ex. '012345' or '543210' or '345120'). 

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

[Back to Portfolio](./)
