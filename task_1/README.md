# Cipher Complexity Overview

| Cipher              | Complexity Type | Description                                                                                                   | Time Complexity       | Space Complexity       |
|---------------------|-----------------|---------------------------------------------------------------------------------------------------------------|-----------------------|------------------------|
| **Playfair Cipher**  | Substitution    | The Playfair cipher encrypts pairs of letters using a 5x5 matrix. It requires preprocessing for matrix creation and then applying substitution rules to digraphs. | **Encryption:** \(O(n)\)  | \(O(1)\) (constant space for the matrix)   |
|                     |                 |                                                                                                               | **Decryption:** \(O(n)\) |                        |
| **Hill Cipher**      | Substitution    | The Hill cipher uses matrix multiplication for encryption and decryption, requiring matrix inversion during decryption. | **Encryption:** \(O(n^2)\)  | \(O(n^2)\) (for matrix storage) |
|                     |                 |                                                                                                               | **Decryption:** \(O(n^3)\) (due to matrix inversion) |                        |
| **Vigenère Cipher**  | Substitution    | The Vigenère cipher applies a key to each letter of the plaintext, rotating through the key letters cyclically. It uses modular arithmetic for encryption and decryption. | **Encryption:** \(O(n)\)  | \(O(k)\) (where \(k\) is the key length)  |
|                     |                 |                                                                                                               | **Decryption:** \(O(n)\) |                        |


# Hybrid Cipher: Hill Cipher + Columnar Transposition Cipher

This repository implements a **Hybrid Cipher** combining the **Hill Cipher** and the **Columnar Transposition Cipher** to provide enhanced encryption. The hybrid approach first applies the Hill Cipher (a substitution cipher) and then applies the Columnar Transposition Cipher (a transposition cipher).

## Overview:

### Hill Cipher
The Hill Cipher is a classical substitution cipher that encrypts data using linear algebra. It uses a square matrix (key matrix) to perform encryption and decryption.

### Columnar Transposition Cipher
The Columnar Transposition Cipher is a transposition cipher that reorders the letters in the plaintext according to a keyword. It breaks the message into rows and reads it in a different order based on the keyword.

### Hybrid Cipher
This hybrid cipher combines the Hill Cipher (substitution) and Columnar Transposition Cipher (transposition) to encrypt data more securely. The process is as follows:

1. **Step 1**: Encrypt the plaintext using the Hill Cipher (substitution).
2. **Step 2**: Encrypt the resulting ciphertext using the Columnar Transposition Cipher (transposition).

To decrypt, the reverse process is followed:
1. **Step 1**: Decrypt the ciphertext using the Columnar Transposition Cipher.
2. **Step 2**: Decrypt the result using the Hill Cipher.

## Code Explanation:
### Hill Cipher
1.The Hill Cipher function encrypts and decrypts a message using a 3x3 key matrix.<br>
2.The hill_encrypt() function transforms the plaintext into numerical equivalents, applies matrix multiplication with the key matrix, and produces the ciphertext.<br>
3.The hill_decrypt() function works similarly but uses the inverse of the key matrix to decrypt the ciphertext.<br>
### Columnar Transposition Cipher
1.The Columnar Transposition function encrypts and decrypts the message by rearranging characters in columns, according to a given keyword.<br>
2.The columnar_transposition_encrypt() function organizes the plaintext into rows and reorders the columns according to the keyword.<br>
3.The columnar_transposition_decrypt() function reverses the column reordering process and reconstructs the original plaintext.<br>
### Hybrid Cipher
1.The hybrid_encrypt() function first applies Hill Cipher encryption to the plaintext and then applies the Columnar Transposition encryption to the resulting ciphertext.<br>
2.The hybrid_decrypt() function first reverses the Columnar Transposition encryption and then decrypts the result using the Hill Cipher.<br>

## Requirements:
1.NumPy: Used for matrix operations, such as matrix multiplication and inversion in the Hill Cipher implementation.<br>
2.string: Part of Python's standard library, used to map characters to numerical equivalents (A=0, B=1, ..., Z=25).<br>

## How to Run:
This file could be run using Google Colab. The link to the code is <a href="https://colab.research.google.com/drive/1iudgOSvICNU1LLy0mPqyu7ahK-_nIZbQ">here</a>
