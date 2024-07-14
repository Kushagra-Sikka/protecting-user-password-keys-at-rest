# Protecting User Password Keys at Rest (on the Disk)

## Project Description

Protecting User Password Keys at Rest is a Python-based application that encrypts files and directories using AES-256 encryption. It securely stores the encryption keys by protecting them with user passphrases and ensures safe retrieval and decryption.

## Features

1. **File/Directory Encryption**: Encrypts a user-chosen file or directory using AES-256 with a randomly generated File Encryption Key (FEK).
2. **Key Protection**: Stores the FEK in a separate file protected by a user passphrase.
3. **Secure Storage**: Ensures that neither the user passphrase nor the FEK is stored in plain text.
4. **Authentication and Decryption**: Retrieves and decrypts the file using the user passphrase to decrypt the FEK.

## Getting Started

### Prerequisites

- Python 3.x
- Required Python libraries (install via `pip`)

### Installation

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/Kushagra-Sikka/protecting-user-password-keys-at-rest.git
   cd protecting-user-password-keys-at-rest

2. **Install Dependencies:**
   ```bash
   pip install cryptography

## Usage

### Encrypt a File or Directory

1. **Encrypt using a random File Encryption Key (FEK).**
2. **Protect the FEK with a user passphrase.**

```bash
python encrypt.py --file <path_to_file_or_directory> --passphrase <user_passphrase>
   
