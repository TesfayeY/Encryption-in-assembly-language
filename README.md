# Encryption-in-assembly-language
The provided assembly code is an encryption and decryption program written in x86 assembly language. It performs a simple encryption and decryption process using a predefined key (array of bytes) to perform an exclusive-OR (XOR) operation with the input text.
Here's a breakdown of what the code does:

InputTheString Procedure:

Displays a prompt for the user to input plaintext.
Reads the input string into the buffer.
Saves the length of the input string.
DisplayMessage Procedure:

Displays the encrypted or decrypted message stored in the buffer.
TranslateBuffer Procedure:

Encrypts or decrypts the string by performing an XOR operation between each byte of the input text and the corresponding byte in the encryption key.
The key is an array of bytes ('z','^','?','>','7','~').
It XORs each byte of the input text with the respective byte in the key.
If the end of the key array is reached during the encryption/decryption process, it resets to the beginning of the key array.
Main Procedure:

Calls InputTheString to get user input.
Calls TranslateBuffer to encrypt the text.
Displays the encrypted message.
Calls TranslateBuffer again to decrypt the encrypted text.
Displays the decrypted message.
Note: The encryption and decryption here rely on a simple XOR operation with a fixed key. This XOR cipher is straightforward and can be easily broken with various cryptographic attacks. This code is for educational purposes and should not be used for secure encryption purposes.
