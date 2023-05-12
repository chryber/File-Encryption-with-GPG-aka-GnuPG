# File Encryption with GPG using Linux Mint

<h2> 🔦 Intro </h2>
Getting hands on with GPU and file encryption. Here I will be going through the simple steps to use this powerful tool in my Linux Mint VM.

<h2>🔩 Utlities Used</h2>

- VMWare WorkStation Player 17
- Linux Mint 21.1 "Vera"

<h2>♻️ The Process</h2>

- Boot up VMWare and starting the VM.
  ![GPG-LM](https://github.com/chryber/File-Encryption-with-GPG-aka-GnuPG/assets/121698544/0141ca29-885a-4224-ac37-059568089a30)
  
 
- Open the terminal and creating a file with sensitive data that is stored on the Desktop. 
  ![GPG-filecreation](https://github.com/chryber/File-Encryption-with-GPG-aka-GnuPG/assets/121698544/b96f72ca-e87b-4920-9798-27ab73ac3819)
  
- GPG comes installed on Linux so no installation of a package is needed. Proceed in using the command to encrypt the file. Notice that the data shows when the plaintext file is               concatenated as opposed to concatenating the encrypted file. Note: I entered my user login password to encrypt.
-         gpg -c filename.txt
  ![GPG-encryptedfile](https://github.com/chryber/File-Encryption-with-GPG-aka-GnuPG/assets/121698544/b5484cbd-a497-4f99-89a3-27eba7e01644)

- Using the same command but replacing -c with -d reveals the encryption algorithm (AES256.CFB) as well as the original contents of the file. 
-         gpg -d filename.txt
  ![GPG-encryption2](https://github.com/chryber/File-Encryption-with-GPG-aka-GnuPG/assets/121698544/12fdc971-5709-4b62-8ef9-f7a1d1583b1c)
