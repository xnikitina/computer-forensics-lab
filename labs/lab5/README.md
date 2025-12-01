# 🧪 Lab 5 – Handle Evidence Data

## 📖 Scenario
After concluding an investigation, a junior investigator submitted evidence files to the court.  
The judge dismissed the case due to poorly handled evidence and improperly presented data.  
This highlights the importance of correctly handling forensic evidence and presenting it in a viable manner.  
In this lab, you will learn how to use **FTK Imager** to examine and manage evidence files.

---

## 🎯 Objectives
- Learn how to add and analyze forensic image files using FTK Imager.  
- Explore the evidence tree to view folders and files.  
- Identify and inspect deleted files within an image.  
- View file properties, hex values, and text values.  
- Export deleted files for further forensic analysis.  

---

## 🔧 Tool Explained
- **FTK Imager** → A forensic imaging and analysis tool used to:
  - Add evidence items such as disk images.  
  - Display file system structures and contents.  
  - Recover deleted files marked within the image.  
  - View file properties, hex values, and text values.  
  - Export files for deeper investigation while preserving integrity.  

---

## 🖥️ Lab Environment
- Windows system with **FTK Imager** available.  
- Evidence image file: `Windows_Evidence_001.dd`.

---

## 📝 Steps/Tasks

### 1. Add Evidence Item
- Launch **FTK Imager**.  
- Go to **File → Add Evidence Item...**.  
- Select **Image File** as the source type.  
- Browse to `Windows_Evidence_001.dd` and add it.  
- The image contents appear in the **Evidence Tree**.

### 2. Explore Evidence Tree
- Expand **Evidence [NTFS] → [root]**.  
- Select the **images** folder.  
- Click on any image file to view its contents.

### 3. Identify Deleted Files
- Scroll through the file list.  
- Files marked with an **X icon** are deleted files.  
- Select a deleted file and open the **Properties** tab to view metadata.

### 4. View File Data
- Click **HEX** to view raw hex values of the file.  
- Click **TEXT** to view text values of the file.  

### 5. Export Deleted Files
- Right‑click on a deleted file and select **Export Files...**.  
- Choose a destination folder (e.g., Desktop).  
- Confirm the export and verify the file at the chosen location.

### 6. Finalize
- Close all open windows.  
- Document your findings: which files were intact, deleted, or suspicious.  

---

## ✅ Outcome
By completing this lab, you have:  
- Learned to handle forensic evidence using FTK Imager.  
- Viewed and analyzed file system contents from a disk image.  
- Identified deleted files and exported them for further investigation.  
- Preserved evidence integrity while preparing data for court presentation.

