# AES256
Encrypt/Decrypt files using AES256 ECB PKCS#7

EXAMPLE:
```
C:\Users\User\aes256>g++ -Wall -Werror AES256.cpp -o aes256

C:\Users\User\aes256>aes256
This program encrypts/decrypts files
using AES256 encryption with ECB mode of operation
and PKCS#7 padding method

The maximum supported file size is 4GB
Enough RAM is required to load the file
Encrypted files are 1 to 16 bytes larger than the original ones

Choose an option:
        1) Generate random key (DON'T USE, THIS RNG CAN BE EASILY REVERTED)
        2) Load key from file
        3) Type key
1

Loading Source of Entropy       COMPLETE
Generating Keys COMPLETE
Key:
E5 A6 D2 32 DA 3A FE 3A 5F 14 79 F0 02 19 E1 8E
E7 6C 24 59 0F 9A E5 76 DA 14 21 FE CB E3 12 55

Key has been stored in the file key.bin

Enter name of the file to Encrypt/Decrypt:
WARNING: The file will be overwritten
example.mp4

Choose an option:
        1) Encrypt
        2) Decrypt
1

10 bytes have been added to the file to encrypt it
Estimated Encryption time: 8 seconds
Encrypted!
50152880 bytes have been encrypted / decrypted in 8 seconds
File saved on disk

C:\Users\User\aes256>aes256
This program encrypts/decrypts files
using AES256 encryption with ECB mode of operation
and PKCS#7 padding method

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
E5 A6 D2 32 DA 3A FE 3A 5F 14 79 F0 02 19 E1 8E
E7 6C 24 59 0F 9A E5 76 DA 14 21 FE CB E3 12 55

Key has been stored in the file key.bin

Enter name of the file to Encrypt/Decrypt:
WARNING: The file will be overwritten
example.mp4

Choose an option:
        1) Encrypt
        2) Decrypt
2

Estimated Decryption time: 66 seconds
Decrypted!
50152880 bytes have been encrypted / decrypted in 65 seconds
10 bytes have been removed from the decrypted file
File saved on disk
```
