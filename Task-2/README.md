# Key Distribution System

## Overview

This implements a secure key distribution system using:
- Public Key Infrastructure (PKI) for asymmetric encryption (RSA).
- Diffie-Hellman (DH) Key Exchange for establishing shared secrets.
- AES Encryption for securing messages.
- Key Revocation Mechanism to revoke compromised keys.

The system securely distributes symmetric encryption keys while preventing attacks such as man-in-the-middle (MITM) and key compromise.

## Features
- RSA Key Pair Generation for PKI.
- Diffie-Hellman Key Exchange to securely negotiate session keys.
- AES-256 Encryption for encrypting messages.
- Key Revocation System to manage compromised keys.
- Secure Key Storage using PEM format.

## Installation

### Prerequisites
Ensure you have Python 3 installed along with the required dependencies:

pip install cryptography

Usage

1. Generate RSA Keys

2.  Perform Diffie-Hellman Key Exchange
  - The system generates DH parameters and keys for secure symmetric key     exchange.
  - A shared secret is derived securely.

3. Encrypt and Distribute a Symmetric Key
  - A 256-bit AES key is generated.
  - The key is encrypted using RSA before distribution.

4. Encrypt Messages with AES
  Use the generated AES key to encrypt confidential messages.

5. Key Revocation

## Run the Program
This program can be run on Google Colab using this link
https://colab.research.google.com/drive/1ZZxYbK9CRf7OZVQeA9a-KYw5lOqgct7s

## Output
<img width="308" alt="image" src="https://github.com/user-attachments/assets/ceff6795-7f15-4fe6-a6ff-656dc52433ef" />


## Security Measures

- RSA + OAEP Padding for strong asymmetric encryption.

- AES-256 with CBC Mode for secure symmetric encryption.

- PKI-Based Authentication to prevent unauthorized access.

- Key Revocation Mechanism to revoke compromised keys.

## Future Enhancements

- Implement OCSP (Online Certificate Status Protocol) for real-time key revocation.

- Add Digital Signatures for authentication.

- Improve the revocation checking mechanism.



