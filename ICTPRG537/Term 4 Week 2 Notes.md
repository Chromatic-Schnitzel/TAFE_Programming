## What is Encryption:
Encryption is a method used to scramble data, this is usually reversible but can be irreversible if so desired, algorithms 

## Terms:
- Symmetrical: A single key is used to Encrypt and Decrypt data
- Asymmetrical: a public key used to encrypt data, and a private key used to decrypt data
- Hashing: Irreversible encrypting data that cannot be reversed
- s

## Symmetrical Encryption
Symmetrical Encryption is less computationally expensive than Asymmetric and thus faster, it is useful when data is being encrypted on a single system, symmetrical encryption requires 

## Asymmetrical Encryption
Asymmetrical encryption requires a public key and a private key, the public key can be used to encrypt data by a third party that can only by decrypted by the paired private key, asymmetrical 

## Common Uses of Encryption
Asymmetric encryption (especially RSA) is quite slow and not suited to large quantities of data, however it is more secure, furthermore data can be encrypted with a significantly faster

## Hashing
Hashing is not technically classified as encryption as it is a one-way summary of data that cannot be reversed, it can present problems with collisions in shorter key sizes, and outputs

## RNG - Random Number Generation
Computers are able to generate pseudo-random numbers through the use of algorithms, basic forms of random number generation is not advised for Cryptography (E.g. System.Random), CSPRNG also known as Cryptographically Secure Pseudorandom Number Generator uses

# Implementing Encryption

## Text Encoding - Keys
Keys used in Encryption will need to be

## Byte[]



## AES Key
A key should not be memorable, nor should it contain any patterns, typically using a generator is a good idea, furthermore the key will need to be stored