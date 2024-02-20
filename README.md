# twain-brute-force
This is an exercise in you assuming the role of a cryptanalyst and trying to break a crypto-
graphic system that consists of the two Python scripts shown here.
The script ``EncryptForFun.py`` can be used for encrypting a message file and the script
``DecryptForFun.py`` for recovering the plaintext message from the ciphertext created by
the first script. With BLOCKSIZE set to 16, the script EncryptForFun.py produces
the following ciphertext output for a plaintext message that is a quote by **Mark Twain**:
``20352a7e36703a6930767f7276397e376528632d6b6665656f6f6424623c2d30272f3c2d3d2172396933742c7e233f687d2e32083c11385a03460d440c25``

Your job is to both recover the original quote and the encryption key
used by mounting a brute-force attack on the encryption/decryption algorithms.

> [!TIP]  
> The logic used in the scripts implies that the effective key size is only 16 bits when the BLOCKSIZE
variable is set to 16. So your brute-force attack need search through a keyspace of size only 2<sup>16</sup>.
