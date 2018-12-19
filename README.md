# AES256
Encrypt/Decrypt files using AES256 ECB ANSI X9.23

EXAMPLE:
```
C:\Users\User\aes256>g++ -Wall -Werror -O3 AES256.cpp -o aes256

C:\Users\User\aes256>aes256
This program encrypts/decrypts files
using AES256 encryption with ECB mode of operation
and ANSI X9.23 padding method

The maximum supported file size is 4GB
Enough RAM is required to load the file
Encrypted files are 1 to 16 bytes larger than the original ones

Choose an option:
        1) Generate random key (DON'T USE, THIS RNG CAN BE EASILY REVERTED)
        2) Load key from file
        3) Type key
1

Loading Source of Entropy       COMPLETE
Generating Keys                 COMPLETE
Key:
56 57 65 75 4B A9 1F 7E C9 9F 25 EC 3E 46 6B B5
57 DE 37 D2 BB C7 7B 42 F8 A5 62 51 BD BC 29 1A

Key has been stored in the file key.bin

Enter name of the file to Encrypt/Decrypt:
WARNING: The file will be overwritten
example.mkv

Choose an option:
        1) Encrypt
        2) Decrypt
1

5 bytes have been added to the file to encrypt it
Estimated Encryption time: 23 seconds
Encrypted!
1083805680 bytes have been encrypted / decrypted in 23 seconds
File saved on disk

C:\Users\User\aes256>aes256
This program encrypts/decrypts files
using AES256 encryption with ECB mode of operation
and ANSI X9.23 padding method

The maximum supported file size is 4GB
Enough RAM is required to load the file
Encrypted files are 1 to 16 bytes larger than the original ones

Choose an option:
        1) Generate random key (DON'T USE, THIS RNG CAN BE EASILY REVERTED)
        2) Load key from file
        3) Type key
2

Enter the name of the binary file containing the key
key.bin
Key loaded from file key.bin
Key:
56 57 65 75 4B A9 1F 7E C9 9F 25 EC 3E 46 6B B5
57 DE 37 D2 BB C7 7B 42 F8 A5 62 51 BD BC 29 1A

Key has been stored in the file key.bin

Enter name of the file to Encrypt/Decrypt:
WARNING: The file will be overwritten
example.mkv

Choose an option:
        1) Encrypt
        2) Decrypt
2

Estimated Decryption time: 56 seconds
Decrypted!
1083805680 bytes have been encrypted / decrypted in 55 seconds
5 bytes have been removed from the decrypted file
File saved on disk
```
