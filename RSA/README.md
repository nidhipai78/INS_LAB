# RSA Encryption and Decryption
This contains an implementation of the RSA encryption and decryption algorithm. RSA is an asymmetric cryptographic algorithm used for secure data transmission. It works by using two keys: a public key (for encryption) and a private key (for decryption).

## Overview
- RSA is based on the mathematical properties of large prime numbers.
- Public Key: Used for encryption.
- Private Key: Used for decryption.
- Key Generation: Involves choosing two large prime numbers, computing n,𝜙(n) and selecting e and d
- Encryption: The plaintext message is converted into ciphertext using the public key.
- Decryption: The ciphertext is converted back to plaintext using the private key.

## Key Concepts
1.	Public Key (e, n): Used for encryption.
2.	Private Key (d, n): Used for decryption.
3.	n: The product of two primes p and q.
4.	ϕ(n): Euler's Totient Function, calculated as (p−1)×(q−1)
5.	e: The encryption exponent, chosen such that gcd⁡(e,ϕ(n))=1
6.	d: The modular multiplicative inverse of eee, calculated modulo ϕ(n)

## Features
Key Generation: Generate public and private keys.<br>
Encryption: Encrypt a message using the public key.<br>
Decryption: Decrypt a message using the private key.<br>

## Requirements
- Python 3.x

## Functions
### gcd(a, b)<br>
Calculates the greatest common divisor of a and b.<br>
### mod_inverse(e, phi)<br>
Calculates the modular inverse of e modulo ϕ(n)<br>
### rsa_encrypt_decrypt()<br>
Main function that handles the RSA encryption and decryption process,including:<br>
•  Input of two prime numbers p and q.<br>
•  Input of the message to encrypt. <br>
•  Calculation of public and private keys. <br>
•  Encryption and decryption of the message.<br>
## How to Use
This program can be run using this link on Google Colab <br>
https://colab.research.google.com/drive/13WDUZexB6dd_RJUqV3yUCZwBHhlr6v65#scrollTo=Ll95XxzjrH34&uniqifier=1

## Output
<img width="245" alt="image" src="https://github.com/user-attachments/assets/9a6c0da3-adea-420e-8018-b69a4b6911f9" />






