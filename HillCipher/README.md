# Hill Cipher
The Hill Cipher is an encryption algorithm that encrypts blocks of text with the help of linear algebra. The repository includes Python code to carry out both encryption and decryption of text using the Hill Cipher technique, using matrix multiplication and modular arithmetic.<br>
## Overview
Hill Cipher is a polygraphic substitution cipher that employs a matrix as the key to encryption. It converts the plaintext to ciphertext through matrix multiplication, where every letter of the plaintext is converted to a number in a vector. The encryption relies on a square matrix, and decryption involves calculating the inverse of the matrix modulo 26.<br>

This project presents Python code that can:
1. Encrypt an input plaintext in a key matrix.
2. Use the inverse of the key matrix to decrypt the ciphertext.

## Requirements
- Python 3.x
- NumPy
  
## How to Use
Install the required dependencies:
    This project uses NumPy for matrix operations.<br>
           pip install numpy<br>
Run the program: 
 - The program could be run using Google Collab. The link for the program is https://colab.research.google.com/github/nidhipai78/HillCipher/blob/main/Hill_Cipher.ipynb

- This program can also be run using GitHub Codespaces using the file HillCipher.ipynb

## Usage
### Input
<img width="394" alt="image" src="https://github.com/user-attachments/assets/2009215b-795b-40ae-a505-7e2844a6894e" />

### Output
<img width="308" alt="image" src="https://github.com/user-attachments/assets/d4aa1ff5-9415-47ba-8738-14606b6838fc" />

## How It Works
The decryption and encryption procedure of the Hill Cipher relies on matrix multiplication:
1. **Encryption**: The plaintext character is replaced by a vector of numbers (A=0, B=1,., Z=25). This vector is multiplied by the key matrix. The resulting vector is translated back into letters to create the ciphertext.
2. **Decryption**: The vector form of the ciphertext is obtained. The modular inverse of the key matrix (mod 26) is computed and applied to the vector to decrypt it back to the original plaintext.

### Steps:
1. Represent the plaintext in numerical form.
2. Pad the plaintext so its length is a multiple of the key matrix size.
3. Multiply the numeric value of the plaintext by the key matrix.
4. Transform the result back into text as ciphertext.
5. To decrypt, multiply the vector of ciphertext by the inverse of the key matrix modulo 26.

