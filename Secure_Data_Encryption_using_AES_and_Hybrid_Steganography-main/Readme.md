Secure Data Transfer Using Cryptography and Hybrid Steganography

This project implements secure data transfer by combining cryptographic techniques (AES and RSA) with hybrid steganography (using DWT and LSB). The system ensures that sensitive information is encrypted and covertly embedded within images, providing robust protection against unauthorized access during online transactions.

Project Overview

	•	Objective: To provide secure transmission of sensitive data using cryptography for encryption and hybrid steganography to conceal the data within images.
	•	Key Features:
	•	AES/RSA Encryption: Encrypts user data to ensure privacy.
	•	2D DWT & LSB Steganography: Embeds encrypted data into a carrier image for secure transmission.
	•	User Authentication: Ensures that only authorized users can decrypt the message.
	•	Data Compression: Uses LZW algorithm to optimize encryption and decryption efficiency.

Components

Cryptography

	•	AES (Advanced Encryption Standard): Symmetric key encryption algorithm used for encrypting sensitive data.
	•	RSA (Rivest–Shamir–Adleman): Asymmetric key encryption algorithm for secure key sharing.

Steganography

	•	Discrete Wavelet Transform (DWT): Decomposes an image into sub-bands (LL, LH, HL, HH) for embedding data.
	•	Least Significant Bit (LSB): Embeds encrypted data in the least significant bits of the carrier image.

Algorithms

	1.	AES Encryption and Decryption:
	•	Encrypts and decrypts data using symmetric keys.
	2.	RSA Encryption and Decryption:
	•	Secures key exchange using asymmetric keys.
	3.	DWT Steganography:
	•	Decomposes carrier images into sub-bands for embedding.
	4.	LSB Encoding:
	•	Embeds encrypted data in the carrier image’s least significant bits.

Requirements

	•	Python 3.x
	•	Libraries:
	•	numpy
	•	pywavelets
	•	matplotlib
	•	PIL (for image processing)
	•	pycrypto (for RSA encryption)

Usage

	1.	Encrypting the Message:
	•	Run the AES/RSA encryption to generate the cipher text.
	•	Embed the cipher text using DWT & LSB steganography in a carrier image.
	2.	Decrypting the Message:
	•	Extract the cipher text from the steganography image.
	•	Use AES/RSA decryption to retrieve the original message.
Expected Outcomes

	•	Ensures data confidentiality and security during transmission.
	•	Prevents unauthorized access and enhances the efficiency of encryption and decryption.
	•	Uses image steganography to avoid detection by attackers.

Future Work

	•	Explore more advanced encryption techniques.
	•	Integrate machine learning to enhance message detection and security.
