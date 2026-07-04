# AES-128 ECB Encryptor
This program is a minimal implementation of AES-128 encryption using ECB mode written for educational purposes to see how AES works internally. It is not a production ready cryptographic tool. 

## Usage
The program reads everything from stdin and writes ciphertext to stdout: 

**Input**
- The first 16 bytes of stdin are used as the AES-128 key.
- The remaining bytes are the plaintext to encrypt. 
- Example: F4C020A0A1F604FD343FAC6A7E6AE0F9 for the key written in hexadecimal, and the block to encrypt F295B9318B994434D93D98A4E449AFD8.

**Output**
- Standard output contain for each block the encryption of that block in the same format as the input.
- Example: output from the above example in hexadecimal is 52E418CBB1BE4949308B381691B109FE.

To run simply use, 
```bash
python3 aes.py < input.bin > output.bin
```