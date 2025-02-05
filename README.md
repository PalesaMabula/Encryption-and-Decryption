# Encryption and Decryption Tool

## Description
This project is a secure file encryption and decryption tool designed to protect sensitive data. It enables users to encrypt and decrypt PowerPoint slides (.pptx), images (.png, .jpg, etc.), and compressed ZIP files using the Advanced Encryption Standard (AES) algorithm. By leveraging the **PyCryptodome** library, the tool ensures robust security for confidential files, making it ideal for secure data storage and transmission.

## Overview
This project is a command-line-based encryption and decryption tool that ensures the security and integrity of files. It supports encryption and decryption of PowerPoint slides (.pptx), images (.png, .jpg, etc.), and compressed ZIP files. The tool leverages the **Advanced Encryption Standard (AES)** algorithm and utilizes the **PyCryptodome** library for cryptographic operations.

## Features
- Encrypts and decrypts PowerPoint slides, images, and ZIP files.
- Uses **AES-256 encryption** for strong security.
- Command-line interface (CLI) for ease of use.
- Ensures data confidentiality and integrity.

## Technologies Used
- **Programming Language**: Python
- **Cryptographic Library**: PyCryptodome
- **Algorithm**: AES (Advanced Encryption Standard)

## Installation
Ensure you have Python installed (Python 3 recommended). Then, install the required dependency:
```sh
pip install pycryptodome
```

## Usage
### Encrypt a File
Run the script and specify the file to encrypt:
```sh
python encrypt.py input_file
```
Example:
```sh
python encrypt.py presentation.pptx
```
This generates an encrypted file with a `.enc` extension.

### Decrypt a File
To decrypt an encrypted file, use:
```sh
python decrypt.py encrypted_file.enc
```
Example:
```sh
python decrypt.py presentation.pptx.enc
```
This restores the original file.

## How It Works
1. The tool reads the input file and generates a secure encryption key.
2. AES-256 encrypts the file content, ensuring confidentiality.
3. The encrypted output is saved with a `.enc` extension.
4. To decrypt, the tool retrieves the key and restores the original file.

## Security Considerations
- Ensure safe storage of encryption keys.
- Avoid sharing sensitive files without proper key management.
- Encrypt large files efficiently by handling them in chunks.



