# PlayfairCipher
This repository provides an implementation of the Playfair Cipher, a classic encryption technique used for encoding and decoding text.

## Introduction
The Playfair Cipher is a digraph substitution cipher. It encrypts pairs of letters (digraphs) instead of single letters.The cipher uses a 5x5 matrix filled with letters of the alphabet, where each letter appears only once. The matrix is created using a keyword, which helps in determining the positions of the letters.<br>

## Playfair Cipher Rules:
1.A 5x5 matrix is created using a keyword and the remaining letters of the alphabet (excluding J, which is combined with I).<br>
2.If a digraph contains the same letter twice (e.g., "LL"), an 'X' is inserted between the letters.<br>
3.Depending on the position of the digraph's letters in the matrix, different rules are applied to encrypt or decrypt:<br>
4.If the letters appear in the same row, each letter is replaced by the letter to its right.<br>
5.If the letters appear in the same column, each letter is replaced by the letter below.<br>
6.Otherwise, each letter is replaced by the letter in its row and column that is at the other letter's position.<br>

## Setup and Requirements
- To run the Playfair Cipher implementation on Google Colab, no installation of external libraries is required. 
Click the link here to access and run the code on Google Colab <a href="https://colab.research.google.com/drive/1iMIMhkZICS1WgQRFW01PM7eag1w5JSek">Click Here</a><br>
- This program can also be run using GitHub Codespaces for the file PlayfairCipher.ipynb

## Input and Output
<img width="216" alt="image" src="https://github.com/user-attachments/assets/943684a9-8758-45aa-80a8-ee9613d7a709" />








