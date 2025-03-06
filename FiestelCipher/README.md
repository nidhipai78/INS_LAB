# Feistel Cipher Implementation

## Overview

This project implements the Feistel Cipher, a symmetric structure commonly used in the design of cryptographic algorithms. The Feistel structure underlies many block ciphers, including DES (Data Encryption Standard).

## Features

- Customizable number of encryption rounds

- Symmetric encryption and decryption

- Key-based encryption

- Modular round function

## Requirements
- Python 3.x

## How To Run
You can directly run using GitHub Codespaces for the file FiestelCipher.ipynb or using this <a href="https://colab.research.google.com/drive/1J7hPEXTpCcv7pSiQo8pXUkb_c5EnhPzG"> Google Collab link.



## Usage
### Input
<img width="285" alt="image" src="https://github.com/user-attachments/assets/c993cde7-8cb1-4181-b3f6-3ee8f4c2e2a5" />

<img width="422" alt="image" src="https://github.com/user-attachments/assets/1561712e-5211-44cc-9b23-893e43c8a405" />

### Output

<img width="453" alt="image" src="https://github.com/user-attachments/assets/1ec82bcd-19ec-4c53-b77a-cc131f4ecc1a" />


## How It Works

1.The plaintext is divided into two halves (Left and Right).

2.A round function processes the Right half with the key.

3.The result is XORed with the Left half.

4.The halves are swapped after each round (except the last round).

5.The process is repeated for the specified number of rounds.

6.Decryption follows the reverse process.

## Round Function

The round function is a critical component of the Feistel Cipher. In this implementation, it performs a simple XOR operation between the Right half and a hashed version of the key.

## Configuration

1.Number of rounds

2.Encryption key

3.Round function complexity

## Security Considerations

1.Higher rounds increase security.

2.Use strong, unpredictable keys.

3.Design more complex round functions for enhanced security.
