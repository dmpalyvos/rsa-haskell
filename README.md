# RSA Implementation in Haskell

Project for the course "Introduction to Computer Science" in the National Technical University of Athens.

## Files
rsa-keygen.hs (key creation) 
rsa-encrypt.hs (rsa encryption)
rsa-decrypt.hs (rsa decryption)
RsaLib.hs (helper function)

## Notes
- rsa-keygen creates private and public rsa keys and saves them in the current directory as rsa-rpv.key and rsa-pub.key respectively.
- The public key is formated as (N, e) and the private key as (N, d)
- rsa-encrypt reads a string from stdin and encrypts it using rsa-pub.key. It prints the encrpted text in stdout as a list of integers.
- rsa-decrypt reads a list of integers (encrypted string) from stdin and decrypts it using rsa-prv.key. It prints the cleartext in stdout.

## Example Encryption
```bash
cat cleartext.txt | ./rsa-encrypt > encrypted
```

## Example Decryption
```bash
cat encrypted | ./rsa-decrypt > cleartext.txt
```
