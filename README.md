## DES Encryption Simulator

This DES (Data Encryption Standard) Encryption Simulator is a Python implementation of the DES encryption algorithm. DES is a symmetric key algorithm for the encryption of digital data and was widely used in the past for secure communications.

### Features:
- **Encryption Implementation**: Provides a functioning encryption process based on the DES algorithm.
- **S-box Substitution**: Utilizes S-box substitution, a crucial step in DES encryption, enhancing security.
- **Round-Key Generation**: Incorporates round-key generation to facilitate multiple encryption rounds.
- **Permutation and XOR Operations**: Employs permutation and XOR operations, fundamental to the DES encryption process.

### How to Use:
1. **Input Message**: Define your message as a binary string.
2. **Generate Keys**: Provide the 16 round keys required for the encryption process.
3. **Execute Encryption**: Utilize the `Encrypt` function to encrypt your message using the provided keys.

### Example:
```python
message = "0000000100100011010001010110011110001001101010111100110111101111"

keys = ["000110110000001011101111111111000111000001110010",
        "011110011010111011011001110110111100100111100101",
        "010101011111110010001010010000101100111110011001",
        "011100101010110111010110110110110011010100011101",
        "011111001110110000000111111010110101001110101000",
        "011000111010010100111110010100000111101100101111",
        "111011001000010010110111111101100001100010111100",
        "111101111000101000111010110000010011101111111011",
        "111000001101101111101011111011011110011110000001",
        "101100011111001101000111101110100100011001001111",
        "001000010101111111010011110111101101001110000110",
        "011101010111000111110101100101000110011111101001",
        "100101111100010111010001111110101011101001000001",
        "010111110100001110110111111100101110011100111010",
        "101111111001000110001101001111010011111100001010",
        "110010110011110110001011000011100001011111110101"]

print(Encrypt(message, keys)) # Output: 1000010111101000000100110101010000001111000010101011010000000101
