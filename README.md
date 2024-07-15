# Protecting User Password Keys at Rest (on the Disk)

## Project Description

Protecting User Password Keys at Rest is a Python-based application that encrypts files and directories using AES-256 encryption. It securely stores the encryption keys by protecting them with user passphrases and ensures safe retrieval and decryption.

## Features

1. **File/Directory Encryption**: Encrypts a user-chosen file or directory using AES-256 with a randomly generated File Encryption Key (FEK).
2. **Key Protection**: Stores the FEK in a separate file protected by a user passphrase.
3. **Secure Storage**: Ensures that neither the user passphrase nor the FEK is stored in plain text.
4. **Authentication and Decryption**: Retrieves and decrypts the file using the user passphrase to decrypt the FEK.

## Getting Started

## Video Demo

[![Demo Video](videos/thumbnail.png)](videos/example.mp4)

Click the image above to watch the demo video.

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
  
## Project Files

- `project.py`: The main Python script that implements the encryption, key storage, and decryption functionalities.


## Usage

### Encrypting a File or Directory
1. Open a terminal or command prompt.

2. Navigate to the project directory where you cloned the repository.

3. **Run the Script**: 
    ```sh
    python3 project.py
    ```

4. **Choose the Encryption Option**: Follow the on-screen prompts to select the option for encrypting a file or directory.

5. **Select the File/Directory**: Provide the path to the file or directory you wish to encrypt.

6. **Enter a Passphrase**: Input a passphrase that will be used to protect the encryption key.

7. **Complete Encryption**: The application will encrypt the selected file or directory and store the encryption key securely.

### Decrypting a File or Directory
1. Open a terminal or command prompt.

2. Navigate to the project directory where you cloned the repository.

3. **Run the Script**: 
    ```sh
    python3 project.py
    ```

4. **Choose the Decryption Option**: Follow the on-screen prompts to select the option for decrypting a file or directory.

5. **Select the File/Directory**: Provide the path to the encrypted file or directory.

6. **Enter the Passphrase**: Input the passphrase used during the encryption process.

7. **Complete Decryption**: The application will authenticate the passphrase, retrieve the encryption key, and decrypt the file or directory.
