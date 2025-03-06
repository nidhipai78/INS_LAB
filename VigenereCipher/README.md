# Vigenère Cipher Implementation

## Overview

This project implements the Vigenère Cipher, a method of encrypting alphabetic text using a simple polyalphabetic substitution technique. The cipher uses a keyword to determine the shifting of letters in the plaintext.

## Features

1.Key-based encryption and decryption

2.Case-insensitive processing

3.Supports alphabetic characters only

4.Simple and efficient implementation

## Prerequisites

- Python 3.x

## How To Run

 This program can be run:
 1. Using GitHub Codespaces for the file VigenereCipher.ipynb
 2. Using this <a href="https://colab.research.google.com/drive/1ZclYkipX77ppR4HeBQ43GHhN7psRxcpi">Google Collab link.


## Example
### Input
<img width="359" alt="image" src="https://github.com/user-attachments/assets/7af00860-9825-40d0-92f5-65b113b82ca6" />

<img width="286" alt="image" src="https://github.com/user-attachments/assets/59a11cf1-008d-4ea1-b7ea-bc8cc91c6a93" />


### Output
<img width="272" alt="image" src="https://github.com/user-attachments/assets/f70b1edb-eeac-41b5-b693-215469694a37" />

## How It Works

1.The plaintext is processed letter by letter.

2.Each letter is shifted according to the corresponding letter in the repeating key.

3.The key letter determines the number of positions to shift the plaintext letter.

4.Decryption reverses the process by shifting in the opposite direction.

## Configuration

- Encryption key

- Case-insensitive processing

## Security Considerations

- Longer keys improve security.

- The Vigenère Cipher is vulnerable to frequency analysis and Kasiski examination.

- Avoid short and predictable keys.


