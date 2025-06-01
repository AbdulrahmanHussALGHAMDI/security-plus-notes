# 🛡️ 1.2 – Non-repudiation

📚 Based on Professor Messer – Non-repudiation (7:57)

---

## 🎯 Overview

**Non-repudiation** ensures that someone **cannot deny** performing an action, such as sending a message or signing a document.  
It's a core concept in cybersecurity that provides **proof of origin** and **proof of integrity**.

> 🧠 Think: "You said it — now you can’t deny it."

---

## 🧾 Real-world Example

Signing a contract:
- ✍️ Your signature proves **you agreed**.
- 🧾 Everyone can **verify** it's your signature.
- 🛡️ You **can’t deny** signing it — that's non-repudiation.

---

## 🔐 In Cryptography

Non-repudiation adds:
- ✅ Proof of **data integrity**
- ✅ Proof of **message origin**
- ✅ High assurance of **authenticity**

This is achieved using:
- **Hashing**
- **Digital Signatures**
- **Private/Public Key Pairs**

---

## 🧬 Proof of Integrity

- A **hash** is a fingerprint of data.
- If any part of the data changes, the hash changes.
- Hashing alone shows **if** data changed — but **not who** changed it.

> Example: If a file's hash differs, something has been altered.

---

## ✍️ Creating a Digital Signature

1. **Hash** the original message.
2. **Encrypt** that hash using the **sender’s private key**.
3. Result = **Digital Signature**
4. Send the **plaintext** + **digital signature** together.

```plaintext
Only the sender (who owns the private key) could have signed it.
