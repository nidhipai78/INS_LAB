# DES Key Generation Implementation

## Overview

This project implements the Key Generation Process of the Data Encryption Standard (DES). The DES algorithm is a symmetric-key block cipher widely used for data encryption.

## Features

1.64-bit initial key input

2.Permuted Choice 1 (PC-1) transformation

3.Key splitting into two 28-bit halves

4.Circular left shifts for subkey generation

5.Permuted Choice 2 (PC-2) transformation

6.Generation of 16 round subkeys

## Prerequisites

- Python 3.x

## How It Works

1.The 64-bit key is reduced to 56 bits by applying Permuted Choice 1 (PC-1).

2.The 56-bit key is split into two 28-bit halves.

3.Each half undergoes circular left shifts based on a predefined schedule.

4.The halves are combined and passed through Permuted Choice 2 (PC-2) to produce 48-bit subkeys.

5.This process is repeated for 16 rounds, generating 16 subkeys.

## Configuration

- Initial 64-bit key in hexadecimal format

- Number of rounds (default: 16)


## Example

### Input
<img width="299" alt="image" src="https://github.com/user-attachments/assets/4444ac55-76b5-4a92-8ebd-e26606be0e59" />

### Output
<img width="376" alt="image" src="https://github.com/user-attachments/assets/b536d4e7-ffa2-4e0b-8eef-175dc1919641" />



## Security Considerations

- DES is vulnerable to brute-force attacks due to its small key size.

- Use stronger encryption algorithms like AES for modern applications.

