# Learning-Encryption-and-Decryption-
Learning encryption, decryption, and classical cryptographic techniques as part of my Information Security journey.
# 🔐 Learning Encryption and Decryption

Welcome to my **Learning Encryption and Decryption** repository!

This repository documents my learning journey in **Information Security and Cryptography**. It includes theoretical concepts, classical cryptographic techniques, coding examples, practice questions, and hands-on exercises.

As a university student, I am developing my understanding of encryption and decryption through practical examples and continuous learning.

## 🎯 Learning Objectives

- Understand the fundamentals of encryption and decryption.
- Learn about plaintext, ciphertext, and cryptographic keys.
- Explore classical cryptographic algorithms.
- Practice encryption and decryption using Python.
- Improve logical thinking and problem-solving skills.
- Build a strong foundation in Information Security.

## 📚 Topics Covered

### 1. Basic Cryptography Concepts
- Plaintext and Ciphertext
- Encryption and Decryption
- Cryptographic Keys
- Symmetric and Asymmetric Encryption

### 2. Classical Cryptographic Techniques
- Caesar Cipher
- Monoalphabetic Substitution Cipher
- Playfair Cipher

### 3. Practical Learning
- Alphabet substitution tables
- Encryption and decryption tables
- Step-by-step cipher operations
- Python coding examples
- Practice questions and challenges

---

## 💻 Coding Examples

The following Python examples demonstrate basic encryption and decryption concepts.

### Example 1: Caesar Cipher Encryption

```python
def encrypt(text, shift):
    result = ""

    for char in text:
        if char.isalpha():
            base = ord('A') if char.isupper() else ord('a')
            result += chr((ord(char) - base + shift) % 26 + base)
        else:
            result += char

    return result


message = "HELLO WORLD"
key = 3

ciphertext = encrypt(message, key)

print("Plaintext:", message)
print("Key:", key)
print("Ciphertext:", ciphertext)
```

**Output:**
```text
Plaintext: HELLO WORLD
Key: 3
Ciphertext: KHOOR ZRUOG
```

**Explanation:** Each letter is shifted three positions forward in the alphabet. For example, A becomes D and H becomes K.

### Example 2: Caesar Cipher Decryption

```python
def decrypt(ciphertext, shift):
    result = ""

    for char in ciphertext:
        if char.isalpha():
            base = ord('A') if char.isupper() else ord('a')
            result += chr((ord(char) - base - shift) % 26 + base)
        else:
            result += char

    return result


ciphertext = "KHOOR ZRUOG"
key = 3

plaintext = decrypt(ciphertext, key)

print("Ciphertext:", ciphertext)
print("Decrypted text:", plaintext)
```

**Output:**
```text
Ciphertext: KHOOR ZRUOG
Decrypted text: HELLO WORLD
```

**Explanation:** Each letter is shifted three positions backward to recover the original message.

---

## 📝 Practice Questions

These questions are designed to strengthen my understanding of encryption and decryption.

### Part 1: Theoretical Questions

1. What is cryptography?
2. Define encryption and decryption.
3. What is plaintext?
4. What is ciphertext?
5. What is a cryptographic key?
6. What is the difference between encryption and decryption?
7. What is the Caesar Cipher?
8. What is a monoalphabetic substitution cipher?
9. What is the Playfair Cipher?
10. Why is cryptography important in Information Security?
11. What is the difference between symmetric and asymmetric encryption?
12. Why are classical ciphers not considered secure for modern applications?

### Part 2: Caesar Cipher Practice

**Question 1:** Encrypt `HELLO` using a Caesar Cipher with a shift key of 3.

**Question 2:** Decrypt `KHOOR` using a shift key of 3.

**Question 3:** Encrypt `SECURITY` using a shift key of 5.

**Question 4:** Decrypt `FDHVDU` using a shift key of 3.

**Question 5:** Write a Python program that accepts a message and a shift key from the user and encrypts the message.

### Part 3: Playfair Cipher Practice

1. Create a 5 × 5 Playfair key matrix using the keyword `MONARCHY`.
2. Encrypt `INSTRUMENTS` using the keyword `MONARCHY`.
3. Identify the rules for letters in the same row.
4. Identify the rules for letters in the same column.
5. Explain what happens when two letters form a rectangle in the key matrix.
6. Why are repeated letters handled specially when preparing plaintext?
7. Why are I and J commonly combined in a standard Playfair matrix?
8. Decrypt a Playfair ciphertext using its corresponding key matrix.

*Note: Playfair exercises should follow a clearly specified convention for repeated letters, filler letters, and combining I/J.*

---

## 🧩 Coding Challenges

The following challenges will help me improve my Python programming skills.

### Beginner Level
- Write a program to encrypt a message using the Caesar Cipher.
- Write a program to decrypt a Caesar Cipher message.
- Allow users to enter their own message and key.
- Preserve spaces, numbers, and punctuation during encryption.

### Intermediate Level
- Create a menu-driven encryption and decryption program.
- Implement a monoalphabetic substitution cipher.
- Validate user input and handle invalid keys.
- Write separate functions for encryption and decryption.

### Advanced Practice
- Implement the Playfair Cipher in Python.
- Create a program that encrypts and decrypts messages using a user-provided keyword.
- Test the program with different plaintext messages.
- Compare the behavior of different classical ciphers.

---

## 📖 My Learning Approach

I am learning through:

- Understanding theoretical concepts.
- Solving encryption and decryption questions.
- Writing and testing Python programs.
- Practicing classical cipher techniques.
- Documenting my progress on GitHub.

## 🚀 Future Goals

- Implement more classical cryptographic algorithms.
- Improve my Python programming skills.
- Explore modern cryptographic concepts.
- Understand the role of cryptography in cybersecurity.
- Build educational projects related to Information Security.

## ⚠️ Disclaimer

This repository is intended for **educational purposes only**.

Classical ciphers such as Caesar and Playfair are useful for learning cryptographic principles but are not suitable for protecting sensitive information in modern applications.

## 🌱 Learning in Progress

This repository will grow as I learn new concepts, solve practice questions, and develop more coding examples.

**Learning today, securing tomorrow. 🔐**

