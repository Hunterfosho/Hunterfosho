# Symmertic Cryptography
- Data Encryption Standard (DES)
  - Designed by IBM 
  - Intended to serve as the federal encryption standard
  - Replace untested algorithms used by agencies
  - Enhanced interoperability of communications
- DES uses an encryption operations called the Feistel function for 16 rounds of encryption
- Each Feistel block performs a combonation of substitution and transposition operations
  - Half block of inputs or 32bits
  - Subkey 48bits
- Key facts about DES
  - Symmetric encryption algorithm
  - Block cipher operating on 64 bit blocks
  - Key length of 56 bits
  - Now considered insecure
- 3DES or Triple DES
  - Using the same DES algorithm multiple times to achieve greater security, specifically 3 rounds
    - Keying option 1
      - K1 ≠ K2 ≠ K3
    - Keying Option 2
      - K1 = K3, K1 ≠ K2, K2 ≠ K3
    - Keying option 3 
      - K1 = K2 = K3
  - Double DES is no more secure than DES, due to the meet-in-the-middle attack
- Triple DES is being phased out
- Facts about 3DES
  - Symmetric encryption algorithm
  - Block cipher operationg on 64 bit blocks
  - Effective key length of 112 bits
  - Considered weak
  
#  Advanced Encryption Standard, Blowfish and Twofish
- The Rijndael algorithm won a competition to become the Advanced Encryption Standard
- AES uses substitution and transpostion 
- Symmetric encryption algorithm
- Block cipher operating on 128 bit blocks
- Key length of 128, 192, or 256 bits
- Considered secure

# Blowfish
- Public domain algorithm
- Designed as a DES replacement
- Uses a Fiestel network
- Combines substitution and transposition
- Symmertric encryption algorithm
- Block cipher operating on 64bit blocks
- Key length anywhere between 32 and 448 bits
- No longer considered secure
  
# Twofish
- Designed as a DES replacement
- Placed in the public domain
- Uses a Feistel network
- Combines substitution and transposition
- Symmetric encryption algorithm
- Block cipher operating on 128 bit block
- Key length of 128, 192, or 256 bits
- Considered secure

# RC4
- Symmetric stream cipher to secure network communications
- RC4 trade secret from 1987 until it was disclosed in 1994
- In the public domain

RC4 and Networking
  - Wired Equivalent Privacy (WEP)
  - Wi-Fi Protected Access (WPA)
  - Secure Sockets Layer (SSL)
  - Transport Layer Security (TLS)

RC4 users a pseudorandom keystream
- Intitalized by using a selected encryption key
- Symmetric encryption algorithm
- Stream cipher
- Variable length key between 40 bits and 2048 bits
- Not considered secure

# Cipher Modes
- Cipher Mode
  - Describes how an alogrithm encrypts and decrypts data
- Common Cipher Modes
  - Electronic Code Book (ECB Mode)
  - Cipher Block Chaining (CBC Mode)
  - Counter Mode (CTR Mode) - block cipher that acts more like a stream cipher
  - Galios/Counter Mode (GCM Mode), adds authentication capability
  
# Steganography
 - Steganography
   -  Steganography is the process of hiding information within another file so that it is not visible to the naked eye
   -  Hides large data in plain sight
      -   One of the most common steganography techniques involves hiding text within an image file