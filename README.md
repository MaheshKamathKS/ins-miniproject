# 🔐 Text Encryption-Decryption Tool

## 📌 Overview
**Text Encryption-Decryption Tool** is a web-based application built as a **mini project** for **Information and Network Security**.  
It offers **two modes** of encryption:
- **Simple Encryption** using Monoalphabetic Substitution Cipher
- **Advanced Encryption** using AES-CBC from the Web Crypto API

---

## 📁 File Structure

```
Text Encryption-Decryption
├── index.html
├── encrypt.html              # Advanced Encryption
├── decrypt.html              # Advanced Decryption
├── encryptmono.html          # Simple Encryption
├── decryptmono.html          # Simple Decryption
├── script.js                 # Advanced logic
└── (Background Image via URL)
```

---

## 📄 Files and Components

### 1️⃣ index.html
This is the homepage that provides navigation to all encryption and decryption tools.

**Components**:
- `<div class="container">`: Main content wrapper
- `<h1>`: Heading
- Section Labels: “Simple Encryption” & “Advanced Encryption”
- Buttons: Link to Encrypt / Decrypt pages
- Footer: Project info and credits

---

### 2️⃣ encryptmono.html & decryptmono.html (Simple Encryption)
Uses Monoalphabetic Cipher where the user provides a **key like "boss"**, and it automatically expands into a full cipher alphabet (`bossacdefgh...`).

**Components**:
- Input fields for text and key
- Encrypt/Decrypt button
- Output display
- Internal CSS for styling

**Logic**:
- Generates substitution alphabet from user’s key
- Encrypts/decrypts using that static mapping

---

### 3️⃣ encrypt.html & decrypt.html (Advanced Encryption)
Uses **AES-CBC encryption** via the **Web Crypto API**, storing the encryption key securely in **Local Storage**.

**Functions in script.js**:
- `encrypt()`: Encrypts text using AES-CBC
- `decrypt()`: Decrypts encrypted content
- `getEncryptionKey()`: Fetches or generates encryption key
- `storeEncryptionKey()`: Securely stores encryption key
- Helper: `encryptWithPassphrase()`, `arrayBufferToHex()`, etc.

---

### 4️⃣ script.js
Handles **Advanced Encryption/Decryption** only.

---

## ⚙️ Working Mechanism

### 🔡 Simple Encryption
1. User enters text and a keyword like `"boss"`.
2. A substitution key is generated.
3. Encrypt/Decrypt logic uses fixed mapping of alphabets.
4. Output is shown immediately.

### 🔐 Advanced Encryption
1. User enters plaintext or ciphertext.
2. JavaScript retrieves/generates AES key.
3. Text is encrypted/decrypted using Web Crypto API.
4. Output appears in textarea.

---

## 🛠 Tech Used
- **HTML**: Web structure
- **CSS (Internal)**: Layout, responsiveness, buttons, and background image
- **JavaScript**: Logic for both encryption types
- **Web Crypto API**: Advanced encryption
- **Local Storage**: Stores encryption key (securely)

---

## ▶️ How to Use

1. Clone or download the project files.
2. Open `index.html` in your browser.
3. Click:
   - "Encrypt"/"Decrypt" under **Simple Encryption** for monoalphabetic cipher
   - "Encrypt"/"Decrypt" under **Advanced Encryption** for AES-based crypto
4. Input text and optionally a key (for mono).
5. Get encrypted/decrypted results instantly!

📝 **Note**: Ensure your browser supports Web Crypto API & local storage for advanced features.

---

## 🚀 Scope for Future Enhancement
- Add **server-side key management** for better security.
- Introduce **login system** to associate keys with users.
- Support **multiple encryption algorithms**.
- Add **copy to clipboard** and **QR code** features.

---

## 📚 Mini Project Info
> This website is a **mini project** for the subject **Information and Network Security**.  
> Developed by **Mahesh Kamath K S**  
> **USN**: NNM22IS086

---

Let me know if you want it in `.md` format or need a download-ready version!
