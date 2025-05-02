# AESECB-CPPHollow
Process Hollowing using C++ and AESECB Encryption.

===================================
   C++ Process Hollowing with AES Encryption
===================================

Description:
------------
This project demonstrates process hollowing in a 64-bit Windows environment using a 32-bit Notepad process. The payload (Executor.exe) is encrypted using AES (ECB mode) and injected into the suspended Notepad process after decryption.

Main Features:
--------------
- AES encryption/decryption using Crypto++ library (ECB mode)
- Secure file read/write for encrypted payloads
- Process hollowing of 32-bit Notepad.exe
- Manual memory allocation and payload injection
- Thread context manipulation via Wow64GetThreadContext / Wow64SetThreadContext

File Structure:
---------------
- payloads\Executor.exe         -> The original payload
- enc\Executor.enc              -> Encrypted version of the payload
- bin\decrypted_payload.bin     -> Decrypted payload for debugging
- main.cpp                      -> Main source code for encryption and injection

Requirements:
-------------
- Windows x64 (WOW64 support required)
- Visual Studio (with C++ compiler)
- Crypto++ library
- Run with Administrator privileges

AES Key:
--------
"Sixteen byte key"

Note: This key is hardcoded for demonstration only.
Avoid using ECB mode or static keys in real applications.

Disclaimer:
-----------
This code is intended strictly for educational and research purposes.
Do NOT use this software against machines you do not own or operate without permission.

Created by: [Your Name or Alias]
Year: 2025

