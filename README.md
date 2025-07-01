# Vigenere Cipher

# How It Works
1. Choose a keyword
Example: KEY

2. Repeat the keyword to match the plaintext length
Plaintext: HELLO

Keyword: KEYKE

3. Encrypt each letter
Each letter of the plaintext is shifted by the value of the corresponding letter in the keyword:

A = 0, B = 1, C = 2, ..., Z = 25

For HELLO and KEYKE:

Plaintext	H	E	L	L	O
Keyword	K	E	Y	K	E
Shift	10	4	24	10	4
Cipher	R	I	J	V	S

Encrypted Text: RIJVS

# Decryption
To decrypt, just reverse the shift:

Subtract the keyword letter's value from the ciphertext letter's value.

# Security
The Vigenère cipher was once considered very secure, but it can be broken with frequency analysis and known-plaintext attacks. It's more secure than Caesar ciphers, but not suitable for modern use.
