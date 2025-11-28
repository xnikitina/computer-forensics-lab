# 🧪 Lab 2 – Perform Hash or HMAC Calculations

## 📖 Overview
This lab demonstrates how to compute hash values and HMACs using **HashCalc**, and how to verify suspicious files against the **VirusTotal** malware database.  
Hashing produces a fixed‑length string (digest) that uniquely represents data. Investigators use hashes to check file integrity and detect malware traces.

---

## 🔧 Tools Explained
- **HashCalc** → A lightweight tool that calculates hash values and checksums for files or text strings using multiple algorithms. It can also compute HMACs (Keyed‑Hash Message Authentication Codes).  
- **VirusTotal** → An online service that scans files or hash values against dozens of antivirus engines. By submitting a hash, investigators can quickly see if a file is recognized as malicious.

---

## 📚 Common Algorithms
- **MD2, MD4, MD5** → Early message digest algorithms; MD5 is widely used but cryptographically broken.  
- **SHA‑1, SHA‑256, SHA‑384, SHA‑512** → Secure Hash Algorithms; SHA‑256 and above are considered strong.  
- **RIPEMD‑160** → Alternative secure hash function.  
- **PANAMA, TIGER** → Less common cryptographic hash functions.  
- **ADLER32, CRC32** → Checksums used for error detection, not cryptographic security.  
- **eDonkey/eMule** → Hashes used in peer‑to‑peer file sharing networks.  
- **HMAC** → Hash‑based Message Authentication Code; combines a secret key with a hash function to verify both integrity and authenticity.

---

## 🎯 Objectives
- Compute hashes of files and text strings.  
- Generate HMAC values using keys.  
- Verify suspicious files by searching their hash values on VirusTotal.  

---

## 🖥️ Lab Environment
- Windows system with **HashCalc** installed.  
- Web browser with internet access.  
- Sample evidence files (e.g., `Kitty.jpg`, `Infected.pdf`).  

---

## 📝 Steps

### 1. Select a File for Hashing
- Open **HashCalc**.  
- In **Data Format**, choose **File**.  
- Select a sample file (e.g., `Kitty.jpg`).  

### 2. Compute Hash Values
- Ensure the **HMAC** box is unchecked.  
- Select desired algorithms (e.g., MD5, SHA‑256, SHA‑512).  
- Click **Calculate**.  
- HashCalc displays the computed hash values for the file.  

### 3. Compute HMAC Values
- Check the **HMAC** box.  
- In **Key Format**, choose **Text String** or **Hex String**.  
- Enter a key (e.g., `test`).  
- Select algorithms (e.g., MD5, SHA‑1, SHA‑512, PANAMA).  
- Click **Calculate**.  
- HashCalc displays the HMAC values for the file.  

### 4. Hash a Text String
- In **Data Format**, select **Text String**.  
- Enter sample text (e.g., `Hello David, how have you been?`).  
- Uncheck **HMAC**.  
- Select algorithms and click **Calculate**.  
- HashCalc displays the hash values for the text.  

### 5. Verify a Suspicious File with VirusTotal
- In HashCalc, select **File** and choose `Infected.pdf` from the evidence folder.  
- Calculate its **MD5** hash (other algorithms may also be selected).  
- Copy the MD5 hash value.  

### 6. Search Hash on VirusTotal
- Open a web browser and go to [VirusTotal](https://www.virustotal.com/gui/home/search).  
- Paste the MD5 hash into the search field and press **Enter**.  
- VirusTotal checks the hash against its database of antivirus engines.  
- Review the results:
  - If multiple engines detect the file as malicious → the file is unsafe.  
  - If no detections → the file may be clean (but further analysis is recommended).  

### 7. Finalize
- Close HashCalc and the browser.  
- Document the hash values and VirusTotal results for reporting.  

---

## ✅ Outcome
By completing this lab, you have:  
- Learned to compute hashes and HMACs using HashCalc.  
- Understood the role of different hash algorithms.  
- Practiced verifying suspicious files against VirusTotal.  
