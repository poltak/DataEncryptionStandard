DataEncryptionStandard
======================

_Co-authored by Hoi Kit Goodwin Lam._
A complete JavaSE 7 implementation of the Data Encryption Standard as specified in FIPS 46-3
(see http://csrc.nist.gov/publications/fips/fips46-3/fips46-3.pdf).

###DES Class
Main DES class, handling the overall logic of the standard. Allows standard DES encryption and
decryption options while also supporting cipher-block chaining mode encryption and decryption
(see https://en.wikipedia.org/wiki/Block_cipher_mode_of_operation#Cipher-block_chaining_.28CBC.29).

###FeistelFunction Class
Handles the main logic involving the F-Function, including expansion, key mixing, substitutions
and permutation. Not intended for use by outside classes.

###RoundKeyGenerator Class
Handles all logic relating to generating all the round-keys out of the 56 bit input key. Not intended
for use by outside classes.