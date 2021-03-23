

## Problem

</br>
Secure Internet Communication
</br>
</br>

* Secure = Confidential and Integral(Verified Recipient)
</br>
</br>
* Confidential = Cryptography
* Integral(Verified) = Signatures (Cryptography)

</br>
</br>

---

## Hacker in the Network

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

## Menti First Question

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

## Asymmetric Encryption with key Exchange

👩‍💻🗝️ <--------------------------- 🏦
</br>
👩‍💻🔩  -------🔒🔩🦹-------> 🔑🏦
</br>
👩‍💻🔩 <---------🦹----------> 🔩🏦

</br>
🗝️ = public key
</br>
🔑 = private key
</br>
🔩 = symmetric key
</br>
🔒🔩 = encrypted symmetric key

---

## Asymmetric Encryption with key Exchange

👩‍💻🗝️ <--------------------------- 🏦
</br>
👩‍💻🔩  -------🔒🔩-------> 🔑🏦
</br>
👩‍💻🔩 <-------------------> 🔩🏦

</br>
🗝️ = public key
</br>
🔑 = private key
</br>
🔩 = symmetric key
</br>
🔒🔩 = encrypted symmetric key

---

## Signatures

</br>

- Signatures Verify Identity
- Signatures Endorse Something

</br>

![Signature](images/signature.jpeg)

Photo by [Lewis Keegan](https://unsplash.com/@skillscouter?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText) on [Unsplash](https://unsplash.com/s/photos/signature?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText)

---

## History of Signatures

</br>

- 3000BC-Present - Seals

- 1677 - State of Frauds act

- 1776 - John Hancock

- 2000 - Electronic Signatures Act


---

## Menti Second Question

---

## Signatures Properties

Signatures are 
- Easy to Verify
- Hard to Reproduce
- Endorse something

One Way Transaction

---

## Signatures and Asymmetric Encryption

- Verify identity via encryption
- I have the key but you have to send me a non-reproducible lock
- key = public key
- non-reproducible lock = encrypted hash (private key)


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
## Verify Identity

</br>
</br>
👩‍💻🗝️ <------------------------ 🏦
</br>
</br>
👩‍💻🗝️ <---------🔏---------🔑🏦
</br>
</br>
👩‍💻 --------------------------☑️🏦
</br>
</br>

- 🗝️ = public key
- 🔑 = private key
- 🔏 = message signed with private key

---

## Hacker Pretender

</br>
</br>
👩‍💻🗝️ <------------------------ 🦹🏦
</br>
</br>
👩‍💻🗝️ <---------🔏🦹---------🔑🏦
</br>
</br>
👩‍💻 ---------------☑️🦹-----------🏦
</br>
</br>

- 🗝️ = public key
- 🔑 = private key
- 🔏 = message signed with private key

---
## Starting Point of Trust

- You have to trust something as a starting point
- Lacking a trust anchor creates a recursive issue
- Bob -> Alice -> Kevin
- Kevin is only as Trust worthy as Bob

---

## Public Key Infrastructure

- You have to trust something as a starting point
- We will use certificates to build trust and disperse keys
- 2 birds with one stone
- Certificates contain a public Key and a Signature

---

## Trust Chain

Draw diagram
- How do you know cert is trust worthy?
- That cert will be signed by another cert
- And so on until you either have a cert in the chain you trust or do not

