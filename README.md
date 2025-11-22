## Assignment 5 Group Project - CSC242
## Group 4 Members: Alex Carris, Rene Navarro, & Danielle Able
## Purpose: 
- This program can encrypt or decrypt a txt file with the Random monoalphabet cipher included in the Cipher.cpp file. 
- For this assignment we were instructed to use the word `FEATHER` as the key/code word.

## How the cipher works

1. Take the keyword: `FEATHER`.
2. Remove duplicate letters: `FEATHR`.
3. Append all remaining unused letters of the alphabet in reverse order.

## Example cipher alphabet:

Plain:  A B C D E F G H I J K L M N O P Q R S T U V W X Y Z  
Cipher: F E A T H R Z Y X W V U S Q P O N M L K J I G D C B  

Uppercase and lowercase letters are preserved. Non-letter characters (spaces,
punctuation, digits) are copied unchanged.

## Files included in this Program
- Cipher.cpp:  source code for the program
- sample_normal.txt:  sample plain/normal text for encryption
- sample_encrypted.txt:  sample encrypted text for decryption

## Building/Compiling

Testing from the project folder:

** Need to download g++ (MinGW-w64) in order to utilize this program **

- Encrypt: ./crypt -kFEATHER sample_normal.txt encrypted.txt 
>> Encrpyts your txt file and pushes the encryption to a txt file named 'encrypted.txt'

- Decrypt: ./crypt -d -kFEATHER sample_encrypted.txt decrypted.txt
>> Decrypts your txt file and pushes the decryption to a txt file names 'decrypted.txt'