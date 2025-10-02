# Cipher Storage App  
**Secure File Share (Cipher Storage App)**  

**Tier:** 3-Advanced  

This application is a **secure file storage and sharing system** designed for mobile devices. The app automatically detects and lists all files stored on a user’s device. The user can then **choose a cipher/encryption method** (e.g., AES, RSA, Blowfish, or custom ciphers) to encrypt a file before sending it to others through any medium (e.g., WhatsApp, Email, Bluetooth).  

The receiver cannot open the file directly. To access it, they must have the **same app installed**. When they try to open the file, the app automatically requests access approval from the sender. If the sender grants permission, the cipher key and method are securely transmitted, allowing the file to be decrypted and opened.  

---

## Purpose of the Application  
- The primary purpose is to enable **confidential file sharing with controlled access**.  
- It ensures **end-to-end security** while giving the sender full control over whether and when a file can be decrypted.  
- It also acts as a **file manager**, displaying all files on the device in an organized manner.  

---

## Resources Needed  
- Knowledge of **cryptographic algorithms** (AES, RSA, etc.).  
- Secure key exchange mechanism (e.g., Diffie–Hellman or RSA-based).  
- Android/iOS file system access APIs.  
- Firebase/Socket-based **real-time communication channel** (for access requests and approvals).  

---

## User Stories  
- [ ] User can view all files stored on their phone within the app.  
- [ ] User can select a file and choose a cipher method to encrypt it.  
- [ ] User can send the encrypted file through WhatsApp, email, or other mediums.  
- [ ] User (receiver) cannot directly open the file unless the app is installed.  
- [ ] User (receiver) can request access from the sender when opening the file.  
- [ ] User (sender) can approve or deny access requests in real-time.  
- [ ] If access is granted, the cipher details are securely shared, and the file is decrypted.  

---

## Bonus Features  
- [ ] User can set **expiry times** for file access (e.g., link expires after 24 hours).  
- [ ] User can allow **one-time access** (receiver can open the file only once).  
- [ ] User can view **logs of access requests** (who requested, when, granted/denied).  
- [ ] App supports **multiple cipher methods** and lets the sender choose.  
- [ ] App includes a **biometric/PIN lock** to access encrypted files.  
- [ ] App integrates with **cloud storage** for encrypted backups.  

---

## Useful Links and Resources  
- [Android File System Access Docs](https://developer.android.com/training/data-storage)  
- [Cryptography with Python](https://cryptography.io/en/latest/)  
- [Firebase Realtime Database](https://firebase.google.com/docs/database)  
- [OWASP Mobile Security Guidelines](https://owasp.org/www-project-mobile-security/)  

---

## Example Projects  
- [Cryptomator](https://cryptomator.org/) – open-source encryption for cloud files.  
- [Tresorit](https://tresorit.com/) – secure encrypted file sharing platform.  
- [OnionShare](https://onionshare.org/) – anonymous file sharing with Tor.  
