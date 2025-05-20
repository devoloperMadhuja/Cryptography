# **Cryptography in C**
A collection of cryptographic algorithm implementations in C, covering classical ciphers and modern encryption techniques.

## **Description**
This repository provides implementations of various cryptographic algorithms in C programming language. Each algorithm includes a brief explanation and an example to help understand its working.

## **Table of Contents**
- [Caesar Cipher](#caesar-cipher)
- [Hill Cipher](#hill-cipher)
- [Affine Cipher](#affine-cipher)
- [Rail Fence Cipher](#rail-fence-cipher)
- [One Time Pad](#one-time-pad)
- [Columnar Transposition Cipher](#columnar-transposition-cipher)
- [Data Encryption Standard (DES)](#data-encryption-standard-des)
- [Advanced Encryption Standard (AES)](#advanced-encryption-standard-aes)
- [RSA](#rsa)
- [Diffie-Hellman Key Exchange](#diffie-hellman-key-exchange)
- [RC4](#rc4)

---

## **Caesar Cipher**
The Caesar Cipher is one of the oldest encryption techniques, shifting letters in the alphabet by a fixed number of positions.

### **Example**
If the shift value is 3:
- Plain text: `HELLO`
- Cipher text: `KHOOR`

---

## **Hill Cipher**
A polygraphic substitution cipher based on linear algebra, using matrix multiplication for encryption and decryption.

### **Example**
If the key matrix is:
 2 3   1 4 
- Plain text: `HI`
- Cipher text: `KM`

---

## **Affine Cipher**
A type of monoalphabetic substitution cipher where each letter is mapped to its numeric equivalent and encrypted using a mathematical function.

### **Example**
If the function is `E(x) = (5x + 8) mod 26`:
- Plain text: `HELLO`
- Cipher text: `AXEEH`

---

## **Rail Fence Cipher**
A transposition cipher that arranges text in a zigzag pattern and reads it row by row.

### **Example**
If the depth is 3:
- Plain text: `HELLO WORLD`
- Cipher text: `HOLELWRDLO`

---

## **One Time Pad**
An encryption technique that is theoretically unbreakable when used correctly.

### **Example**
- Plain text: `HELLO`
- Key: `XMCKL`
- Cipher text: `EQNVZ`

---

## **Columnar Transposition Cipher**
A transposition cipher that rearranges characters based on a predefined column order.

### **Example**
If the key is `4312567`:
- Plain text: `HELLO WORLD`
- Cipher text: `HOLELWRDLO`

---

## **Data Encryption Standard (DES)**
A symmetric-key algorithm that encrypts data in 64-bit blocks using a 56-bit key.

### **Diagram**
![DES Diagram](https://upload.wikimedia.org/wikipedia/commons/8/81/DES-main-network.png)

---

## **Advanced Encryption Standard (AES)**
A symmetric encryption algorithm that operates on blocks of data using keys of 128, 192, or 256 bits.

### **Diagram**
![AES Diagram](https://upload.wikimedia.org/wikipedia/commons/2/27/AES-Encryption-Involution.png)

---

## **RSA**
An asymmetric cryptographic algorithm used for secure data transmission.

### **Example**
- Public key: `(e, n)`
- Private key: `(d, n)`
- Plain text: `HELLO`
- Cipher text: `...`

---

## **Diffie-Hellman Key Exchange**
A method for securely exchanging cryptographic keys over a public channel.

### **Example**
- Public values: `P = 23`, `G = 9`
- Private keys: `a = 4`, `b = 3`
- Shared secret key: `9`

---

## **RC4**
A stream cipher that encrypts data byte by byte using a pseudo-random key stream.

### **Example**
- Plain text: `10011000`
- Key stream: `01010000`
- Cipher text: `11001000`

---

## **Usage**
Clone the repository and compile the C files to test each encryption method.

```sh
git clone https://github.com/your-username/cryptography-in-c.git
cd cryptography-in-c
gcc caesar_cipher.c -o caesar_cipher
./caesar_cipher
