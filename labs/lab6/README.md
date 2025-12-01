# 🧪 Lab 6 – Create a Disk Image File of a Hard Disk Partition

## 📖 Scenario
During a forensic investigation, an investigator accidentally triggered a process that deleted all disk data.  
Fortunately, a forensic copy of the disk had already been created, allowing the investigation to continue.  
This highlights the importance of **always creating a duplicate (disk image) before performing forensic analysis**.

---

## 🎯 Objectives
- Understand how to create a **bit‑by‑bit disk image** of a hard disk partition.  
- Learn to use **R‑Drive Image** for forensic imaging.  
- Preserve evidence integrity by working on the copy instead of the original disk.  

---

## 🖥️ Lab Environment
- Windows 11
- Internet connection with web browser  
- Administrator privileges  

---

## 📝 Steps/Tasks

### 1. Launch R‑Drive Image
- Open **R‑Drive Image**.  
- The main GUI appears.

### 2. Create Image
- Select **Create Image** from the main menu.  
- In the **Partition Selection** window, choose **C:** to image the system partition.  
- Click **Next**.

### 3. Choose Destination
- In the **Image Destination** panel:  
  - Expand *This PC* and select **(C:)**.  
  - The filename is automatically generated.  
  - Select file type: **R‑Drive Image files (*.rdr)**.  
- Click **Next**.

### 4. Start Imaging
- In the **Total Operations List** window, click **Start**.  
- The **Progress bar** shows completion percentage.  
- Imaging may take ~10 minutes depending on disk size.

### 5. Confirm Success
- When finished, a pop‑up confirms: **Image created successfully**.  
- Click **OK**.

### 6. Exit Tool
- Click the three dots in the top‑right corner → **Exit**.  
- Navigate to the **Z: drive** to verify the created image file.  
- Note: Image size depends on used space in the partition.

---

## ✅ Outcome
By completing this lab, you have:  
- Created a forensic disk image of a hard disk partition.  
- Preserved all files, deleted data, slack space, and file system information.  
- Ensured forensic analysis can be performed safely on the copy without risking original evidence.
