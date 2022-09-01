# Encryption   
-  Cryptography is one of the most important controls available to information security professionals. Encryption protects sensitive information from unauthorized disclosure in many different environments and many other security functions depend upon cryptography to work properly
   -  Use of mathematical algorithms to transform information into a form where it's not readable by unauthorized individuals but authorized individuals have the ability to transform it back into its readable form
   -  Encryption, converts information from its plain text form into an encrypted version that is unreadable, known as ciphertext
   -  Decryption, performs the reverse transformation, using an algorithm to transform encrypted information back into plain text form
   -  Algorithm are similar to computer code. often designed to implement the mathematical function

# Symmetric and Asymmetric Cryptography
-   Symmetric encryption algorithms also known as shared secret encryption algorithms, the encryption and decryption operation use the same key
-   Asymmetric encryption algorithms use different keys for encryption and decryption

# Goals of Cryptography
-   Confidentiality
    -   Confidentiality ensures that unauthorized individuals are not able to gain access to sensitive information
        -   Data at Rest - Stored on a hard drive or other storage
        -   Data in Transit - Transmitted over a network connection
        -   Data in Use  - Process actively used in memory
-   Integrity
    -   Integrity - Integrity protects messages against unauthorized modifications
-   Authentication
    -   Authentication - Proof of identity claims
-  Obfuscation  
    -   Making data unintelligible to anyone
        -   Example - Replacing SSN numbers with a unique valve so that its much less sensitive
-   Non-Repudiation
    -   Proving an action was done or performed by an individual in a way that it cannot be denied

# Codes and Ciphers
- Codes
  - A system that substitutes one word or phrase for another; intended to provide secrecy and/or efficiency
     - Example - the 10 code systems used by emgergency personnel
- Ciphers
  - A system that uses mathematical alogrithms to encrypt and decrypt messages
    - Stream Ciphers - Stream ciphers work on one character of the message at a time
    - Block Ciphers -  Work on chunks of the message, known as blocks, at the same time
    - Substitution Ciphers - Change the characters in a message, also called a rotation ciphers
      - Rotation Ciphers start with ROT and then follow the numerical value -
        - Example - The Cipher ROT13 changes the 13 characters in the message
    - Transpositional Ciphers do not change, instead they are rearranged

# Cryptographic Math
- Cryptographic algorithms use the Exclusive Or operation to combine plain text and cipher text with cryptographic keys. The Exclusive Or operation, which is often abbreviated X-O-R or XOR, is a logical operation that is true when one, and only one, of the inputs is true. Let's take a look at the truth table for the XOR operation. Here we have two variables, X and Y, and then the Exclusive Or of those two variables, which is represented by the symbol that you see here on the screen, a plus with a circle around it. If we have two inputs, X and Y, and they're both false, then neither one of those is true and X exclusive or Y is false. If X is true and Y is false, then exactly one of the inputs is true and X exclusive or Y is true. The same thing happens if X is false and Y is true. But if both X and Y are true, the Exclusive Or operation is false because it allows only one of the inputs to be true.

# Crypographic Lifecycle
- The cryptographic lifecycle manages the use of encryption materials over time
  - As cryptographic algrorithms age, they ofen become insecure
  - Researchers discover a flaw or becomes vulnerable to brute force attack 
- 5 stages of the cyrptograhic lifecycle
    - 1. Initiation
    - 2. Development and Acquisition
    - 3. Implementation and Assessment
    - 4. Operations and Maintenance
    - 5. Sunset