## Cryptography

Cryptography = Secrets

![Whispering](https://source.unsplash.com/YLMs82LF6FY/540x360)

Photo by [Sai De Silva](https://unsplash.com/@scoutthecity?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/secret?utm_source=unsplash&amp;utm_medium=referral&amp;utm_content=creditCopyText)

---

## Cryptography Continued

</br>

Cryptography is about **secrets!**

</br>

- Helps you communicate confidentially
- Nations and Militaries used to use it
- Today people use it via browsers and servers

Note:
Now each of our browsers and servers are doing thousands of encryptions/decryptions a day.

---

## Scytale (500-401 BC)

![Cylinder Cryptography Device](https://upload.wikimedia.org/wikipedia/commons/thumb/5/51/Skytale.png/400px-Skytale.png)

"I am hurt very badly help" -> "Iryyatbhmvaehedlurlp"

```
       | I | a | m | h | u |  |
     __| r | t | v | e | r |__|
    |  | y | b | a | d | l |
    |  | y | h | e | l | p |
```

Image/example from [wikipedia](https://en.wikipedia.org/wiki/Scytale)

Note:
Apparently when the Spartan's weren't kicking people into pit's and yelling this is Sparta they were working on some pretty neat cryptography.
It's believe they may have use this device to encrypt and decrypt messages. Two cylinders/skytales with identical diameters would have to be used.
One would wrap a piece of leather around the cylinder and then you would write out your message. Then once you unwrapped the leather it was essentially
encoded since the leather didn't make sense without decryption. The recipient would use their skytale to quickly decrypt the message. So a couple
interesting things to note are that nothing in the original message changed. This message has simply been shuffled this is referred to as transposition cipher.
For those quick to notice patterns will realize that essentially this is taking every fifth letter/character.

---

## Caesar Cipher (100-44BC)

ROT1

| Encrypt | Decrypt |
|---------|---------|
| A -> B  | B -> A  |
| B -> C  | C -> B  |
| C -> D  | D -> C  |
| T -> U  | U -> T  |

So CAT -> DBU -> CAT

Note:
If you have ever heard of a cipher or made one this one is likely it. This involves remapping letters by rotating the alphabet by a certain number of letters.
This is what is referred to as substitution cipher since your substituting notice unlike the previous it's possible none of the original message still exists.

---

## ROT13 Caesar Cipher


![ROT13](https://upload.wikimedia.org/wikipedia/commons/thumb/2/2a/ROT13.png/640px-ROT13.png)


Image/example from [wikipedia](https://en.wikipedia.org/wiki/Scytale)

Note:
The most popular version is ROT13 which rotates the letters by 13. The advantage of this is that since the alphabet is 26 letters the same algorithm/table can be used to encrypt and decrypt.
These algorithms are very easy to break and should not be used for anything that really needs to be kept secret. However, they are useful for an easy introduction into encryption.
Historians believe at the time they were unbreakable.


---

## Notable Events</br></br>

- Al-Kindi, an Arab Mathematician develops frequency analysis(800)</br></br>
- British Intelligence intercepts and decodes Zimmermann Telegram(1917)</br></br>
- Alan Turing develops a machine(Bombe) to decrypt Enigma(1939-1943)</br></br>

Note:
There was continuous developments in cryptography however I want to just focus on the core concepts which were captured by the easier to understand examples.
However, I will just briefly describe some of the other events.
Frequency analysis provides valuable insights into breaking ciphers.
Decoding the Zimmermann Telegram helped to shape American public opinion during WW1 motivitating the US to enter.
Some historians that breaking the Enigma code shortened the war in Europe by as many as two to four years.(https://www.bbc.com/news/technology-18419691)

---

## Modern Cryptography
- [Data Encryption Standard(DES)]() 1977 - unclassified, sensitive information
- [Advanced Encryption Standard(AES)](https://csrc.nist.gov/csrc/media/projects/cryptographic-standards-and-guidelines/documents/aes-development/rijndael-ammended.pdf#page=1) 2001 - Current standard globally for transferring sensitive information
- [Simplified AES](https://www.ime.usp.br/~rt/cranalysis/AESSimplified.pdf) - Variant used for learning

Note: Until the 1960s cryptography was really primarily used by government and more specifically their military.
However, with the advent of the Internet and the need for communicating securely cryptography entered the public domain.

---

## Computing Details

- data = numbers
- spreadsheets, images, videos, letters = numbers
- For example 
  - Z = 90 = 0x5A
  - z = 122 = 0x7A
  - White = 255, 255, 255
- Hex = 0,1,2,3,4,5,6,7,8,9,A,B,C,D,E,F
  - A = 10
  - B = 12
  - ...
  - F = 16

Note:
This means mathematicians can work with these numbers and encrypt anything.

---

## AES Exercise

https://cryptii.com/pipes/text-to-binary
https://cryptii.com/pipes/aes-encryption
https://cryptii.com/pipes/hex-to-text


**AES-256 CBC Encoded Bytes:**

7a b6 4d 5c c2 3c 2f 58 27 a3 b9 9a 1c 3a ef 5b 94 4c d8 8b a5 b0 56 b6 4e c5 71 86 9d 68 7c f1


**Key in Text:**

passwordpasswordpasswordpassword

---

## Hacker in the Network (Recap)

</br>
</br>
👩‍💻 -------✉️🦹-------> 🏦

</br>
</br>

🦹📩 = 💸

---

## Sending key with message 

</br>
</br>
👩‍💻 -------🔑🔒🦹-------> 🏦

</br>
</br>

🦹🔑🔒= 📩
</br>
</br>
🦹📩 = 💸

---

## Pre Shared Key

</br>
</br>
👩🔑 <--> 🔑🏦
</br>
</br>
👩‍💻🔑 -------🔒🦹-------> 🔑🏦

</br>
</br>
🦹 = 😞

---

## Asymmetric Encryption

</br>
</br>
👩‍💻🗝️ <------------------------ 🏦
</br>
</br>
👩‍💻🗝️  -------🔒🦹-------> 🔑🏦

</br>
</br>
🗝️ = public key
</br>
🔑 = private key

</br>
</br>

🦹 = 😞

---

## Hacker's new tricks

</br>
</br>
👩‍💻🗝️ <------------------------ 🦹🏦
</br>
</br>
👩‍💻🗝️  -------🔒🔑🦹🗝️-------> 🔑🏦

</br>
</br>
🗝️ = public key
</br>
🔑 = private key

</br>
</br>

🦹🔑🔒= 📩
</br>
</br>
🦹📩 = 💸
