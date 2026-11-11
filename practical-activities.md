# Practical Demonstrations and Exercises

This page records practical activities described in the supplied Cryptography teaching materials. It should not be read as confirmation that every activity was completed unless supported by session records or photographs.

## 1. OpenSSL file encryption and decryption

The materials guide learners through creating a sample file, encrypting it with OpenSSL, locating the encrypted output and decrypting it with the correct passphrase and matching settings.

The expanded instructor deck includes an AES-256-CBC example using PBKDF2 for passphrase-based key derivation. Learners are prompted to compare the recovered file with the original.

## 2. SHA-256 file hashing

The deck introduces the command:

```bash
openssl dgst -sha256 notes.txt
```

Learners are asked to repeat the hash operation, then change a practice copy of the file and observe that the digest changes. The materials emphasise that a reference digest must itself be trusted for the comparison to be meaningful.

## 3. Caesar cipher

The Caesar cipher is used as an introductory substitution-cipher exercise.

- Choose a shift value, such as +3.
- Move each letter forward to encrypt.
- Move each letter backward to decrypt.
- Apply wraparound at the end of the alphabet.

The slide challenge asks learners to encrypt `CYBER` using +3 and decrypt `FDHVDU` using shift 3. The supplied answer key gives `FBEHU` and `CAESAR`.

The materials explicitly state that Caesar cipher is educational and not suitable for protecting real secrets.

## 4. Wireshark observation: Telnet and SSH

The deck proposes using Wireshark to examine authorised lab traffic or an instructor-provided packet capture. The activity compares Telnet and SSH and asks learners to observe protocol layers and distinguish visible metadata from encrypted payload content.

## Lab safety

Use only instructor-provided sample data, your own lab traffic, or systems for which explicit permission has been granted. Do not capture other people's communications or use real passwords, private keys or confidential files in classroom exercises.
