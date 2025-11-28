# 🧪 Lab 3 – Compare Hash Values of Files to Check their Integrity

## 📖 Scenario
During an investigation, a forensic examiner must verify the integrity of copies of sensitive files.  
To do this, the examiner calculates the hash values of the suspect files and compares them with the pre‑existing hash values of the original files.  
If the values match, the integrity is preserved; if not, the file may have been modified.

---

## 🎯 Objectives
- Generate the **MD5 hash value** of selected files using **MD5 Calculator**.  
- Compare generated hash values with pre‑existing hashes to determine file integrity.  

---

## 🔧 Tool Explained
- **MD5 Calculator** → A simple utility that computes the MD5 hash of files.  
  - It allows investigators to generate a hash for any file.  
  - It also provides a **Compare To** field where you can paste a known hash value.  
  - The tool instantly compares both values and reports whether they match.  
  - This makes it useful for verifying file integrity in forensic investigations.

---

## 🖥️ Environment
- Windows system with **MD5 Calculator** installed.  
- Evidence files.  
- Hash repository file: `Hashes.txt`.  

---

## 📝 Steps/Tasks

### 1. Calculate a Hash Value
- Open **MD5 Calculator**.  
- Click **Add Files** and select `peacesign.jpg` from the evidence folder.  
- Click **Calculate** to generate the MD5 hash.  
- The hash value appears under the **MD5 Value** section.

### 2. Compare Hashes of Friends2.jpg
- Open `Hashes.txt` in the evidence folder.  
- Copy the stored hash value for `Friends2.jpg`.  
- In **MD5 Calculator**, add `Friends2.jpg` and calculate its MD5 hash.  
- Paste the copied hash into the **Verify MD5 Value** field.  
- Click **Compare**.  
- If the values match → the file’s integrity is intact.

### 3. Compare Hashes of Model.png
- Copy the stored hash value for `Model.png` from `Hashes.txt`.  
- In **MD5 Calculator**, add `Model.png` and calculate its MD5 hash.  
- Paste the copied hash into the **Verify MD5 Value** field.  
- Click **Compare**.  
- If the values do not match → the file’s integrity is questionable and requires further investigation.

### 4. Finalize
- Close all open windows.  
- Document your findings: which files matched and which did not.  

---

## ✅ Outcome
By completing this lab, you have:  
- Learned to compute MD5 hashes of files.  
- Compared generated hashes with stored values.  
- Verified file integrity and identified potential modifications.
