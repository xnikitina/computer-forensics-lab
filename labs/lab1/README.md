# 🧪 Lab 1 – Recover Data from a Windows Hard Disk

## 📖 Scenario
A finance manager in a reputable company modifies the financial data of the company and transfers the company’s funds 
to his personal account. In order to conceal the evidence, he permanently deletes the original files from his 
computer using **Shift+Del**. 
Your task as a computer forensic investigator: recover the deleted files using forensic tools.

## 🎯 Objectives
- Learn to use **EaseUS Data Recovery Wizard**.
- Recover permanently deleted files.
- Document recovery process for chain of custody.

## 🖥️ Environment
- Windows 11 (VM or physical)
- Internet connection + admin rights

## 📖 Overview
This lab familiarizes you with the tool **EaseUS Data Recovery Wizard** and helps you understand how to recover files
that have been deleted from a Windows system.

## 📝 Steps/Tasks

**Note:** In this lab, we are considering that the footprint of the investigation is not a major issue.

1. Turn on the Windows 11. 
2. Copy sample files, `Financial Statement Sample.pdf` and `Profit and Loss Statement Sample.xlsx` to some example folder and permanently delete them with **Shift+Del**.
3. Create some other folder **Recovered Files**. (Recovered files or folders should ideally be saved to a different drive, such as an external USB device or cloud storage, rather than the original disk.)
4. Install (if not) and run **EaseUS Data Recovery Wizard**.  
5. In the **Devices and Drives** section select path to folder with deleted sample files  and click **Search for lost Data**.  
6. Navigate to found deleted files `Financial Statement Sample.pdf` and `Profit and Loss Statement Sample.xlsx` and with right‑click select **Preview**.
Note: Full preview is only available in the premium version.
7. Select files in the preview and click **Recover**.
8. In the **Browse for Folder** window, select the **Recovered Files** folder created earlier. 
9. Save recovered files to `Documents/Recovered Files`.
10. A **Recover Complete** window appears → close it.
11. Files are saved to `Documents\Recovered Files`. EaseUS auto‑creates sub‑folders:  `Recovered → Preview`.
12. Navigate manually to:  `Documents\Recovered Files\Recovered\Preview` 
13. Verify recovery and folder structure.  

---

## ✅ Outcome
By completing this lab, you have:

- Practiced recovering permanently deleted files.  
- Verified file integrity using EaseUS Data Recovery Wizard.  
- Documented the recovery process for forensic reporting.  


