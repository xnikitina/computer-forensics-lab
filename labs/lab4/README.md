# 🧪 Lab 4 – View Files of Various Formats

## 📖 Scenario
A network administrator reported the transmission of unknown files across the company’s network after a security breach.  
Investigators discovered that the attacker had hidden the file format to confuse the administrator.  
Using **File Viewer**, they were able to recognize the true format and extract the contents that revealed the attack.

---

## 🎯 Objectives
- Learn how to open and examine files of different formats using **File Viewer**.  
- Understand how to identify suspicious files whose extensions may have been changed.  
- Practice viewing file properties to gather forensic information.  

---

### 🔧 Tool Description – File Viewer
**File Viewer** is a forensic utility that allows investigators to:
- Open files of multiple formats (images, documents, audio, video, text).
- Inspect file contents even if the extension has been changed.
- View file properties and metadata (size, timestamps, author, hidden strings).
- Work in read‑only mode to preserve evidence integrity.

This makes File Viewer efficient for quickly identifying suspicious files, detecting format manipulation, and gathering forensic details without altering the original data.

---

## 🖥️ Environment
- Windows system with **File Viewer** available.  
- Evidence files located in `E:\CHFI-Tools\Evidence Files\Image Files`.  

---

## 📝 Steps/Tasks

### 1. Open an Image File
- Launch **File Viewer**.  
- Go to **File → Open**.  
- Navigate to `E:\CHFI-Tools\Evidence Files\Image Files`.  
- Select `cartoon-article.jpg` and click **Open**.  
- The image opens in the File Viewer window.  
- Go to **File → File Properties** to view metadata such as size, type, and creation date.

### 2. Attempt to Open a Video File
- In **File Viewer**, go to **File → Open** again.  
- Navigate to the evidence folder.  
- Select `520px-Biohazard_symbol_(blue).mp4` and click **Open**.  
- File Viewer attempts to run the file but fails, showing a blank screen.  
- This indicates the file may be corrupt or its extension has been altered.  
- Such files require further forensic investigation.

### 3. Finalize
- Close all open windows.  
- Document your findings:  
  - Which files opened successfully.  
  - Which files failed to open and may be suspicious.  

---

## ✅ Outcome
By completing this lab, you have:  
- Learned to open files of different formats using File Viewer.  
- Viewed file properties to gather forensic metadata.  
- Identified suspicious files that may have been corrupted or tampered with.

