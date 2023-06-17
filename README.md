# 4D-Fractional-Dimension-Lattice-Encryption
4D Fractional Dimension Lattice Encryption


The Fractional Dimension Lattice-based Encryption Algorithm is designed to encrypt and decrypt messages using a lattice structure with fractional dimensions. Here's a breakdown of how the algorithm works:

Lattice Generation: The algorithm starts by creating a lattice structure with specified dimensions (width, height, depth, and time). Each lattice point represents a symbol with associated properties such as a numeric value, a set of colors, and a complexity represented by a bitset.

Message Encryption: To encrypt a message, the algorithm takes the input message and an encryption key. It iterates over each character in the message and performs the following steps:
a. Identifying lattice indices: The algorithm calculates the lattice indices for the current character based on its value and the size of the lattice.
b. Symbol Selection: The algorithm retrieves the lattice symbol corresponding to the calculated indices. It selects a symbol with the highest complexity among all lattice symbols in the lattice structure.
c. Encryption Operation: The algorithm XORs the current character with the encryption key and the modulo 256 of the selected symbol's numeric value. The resulting value is stored as the encrypted character.
d. Delay: The algorithm introduces a random delay before processing the next character to add an element of randomness and security.

Message Decryption: To decrypt an encrypted message, the algorithm takes the encrypted message, the encryption key, and the number of encryption rounds. It performs the following steps:
a. Encrypted Character Extraction: The algorithm iterates over each character in the encrypted message.
b. Symbol Selection: Similar to encryption, the algorithm calculates the lattice indices for the current encrypted character and selects the lattice symbol with the highest complexity.
c. Decryption Operation: The algorithm XORs the encrypted character with the encryption key and the modulo 256 of the selected symbol's numeric value. The resulting value is stored as the decrypted character.
d. Delay: Similar to encryption, the algorithm introduces a random delay before processing the next encrypted character.

Result: After decrypting all characters, the algorithm returns the decrypted message.

The Fractional Dimension Lattice-based Encryption Algorithm combines the properties of the lattice structure, randomness, and encryption key to provide a secure and unique encryption scheme. The inclusion of fractional dimensions allows for a more complex and versatile lattice structure, potentially enhancing the encryption strength and diversity of symbols.
