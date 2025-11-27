# Computer Forensics Lab

## 🔹 Context
Rising cybercrimes such as IP theft, cyberterrorism, and corporate litigation demand forensic investigations.  
Laws and standards define cybercrime, evidence handling, search/seizure, and recovery.  
Investigators must follow strict, repeatable, and documented processes to ensure evidence integrity and legal admissibility.

## 🎯 Lab Objectives
- Recover deleted files from evidence
- Generate hashes and checksum files
- Calculate MD5 values of selected files
- View files in multiple formats
- Analyze evidence and generate an investigative report
- Create a disk image of a hard disk partition

## 🖥️ Lab Environment
- Windows 11 (VM or physical) and Windows Server 2022 VM
- Internet access via web browsers
- Administrator privileges for forensic tools

## 🔍 Investigation Process Overview
- Methodical approach: seize, analyze, and report digital evidence
- Conducted in a Computer Forensics Lab (CFL) equipped with hardware/software tools
- Tools such as EaseUS Data Recovery Wizard, MD5 Calculator, HashCalc enable recovery, duplication, and checksum comparison
- Lab results help determine guilt/innocence and strengthen case integrity

---

## 🧪 Lab Tasks

### Lab 1: Recover Data from a Windows Hard Disk
- Use **EaseUS Data Recovery Wizard** to restore deleted files from a Windows hard disk.
- Document recovered files and note integrity checks.

### Lab 2: Perform Hash/HMAC Calculations
- Use **HashCalc** to generate hash values (MD5, SHA-1, SHA-256).
- Record outputs for later comparison.

### Lab 3: Compare Hash Values
- Use **MD5 Calculator** to verify file integrity.
- Compare generated hashes against known values.

### Lab 4: View Files in Multiple Formats
- Use **File Viewer Lite** and **Adobe Reader** to inspect evidence in different formats.
- Note anomalies or suspicious content.

### Lab 5: Handle Evidence Properly
- Practice evidence handling procedures: documentation, chain of custody, and secure storage.
- Ensure compliance with forensic standards.

### Lab 6: Create a Disk Image
- Use **R-Drive Image** or **FTK Imager** to create a disk image of a hard disk partition.
- Verify image integrity with hash comparison.

---

## 📂 Repository Structure

```text
computer-forensics-lab/
├── labs/
│   ├── lab1/                    # Recover Data from a Windows Hard Disk
│   │   ├── README.md            # Lab description, scenario, objectives, steps
│   │   ├── prerequisites.md     # Requirements (VMs, tools, environment setup)
│   │   └── docs/                # Supporting docs, screenshots, notes
│   ├── lab2/                    # Perform Hash/HMAC Calculations
│   │   ├── README.md
│   │   ├── prerequisites.md
│   │   └── docs/
│   ├── lab3/                    # Compare Hash Values
│   │   ├── README.md            
│   │   ├── prerequisites.md     
│   │   └── docs/                
│   ├── lab4/                    # View Files in Multiple Formats
│   │   ├── README.md
│   │   ├── prerequisites.md
│   │   └── docs/
│   ├── lab5/                    # Handle Evidence Properly
│   │   ├── README.md
│   │   ├── prerequisites.md
│   │   └── docs/
│   ├── lab6/                    # Create a Disk Image
│   │   ├── README.md
│   │   ├── prerequisites.md
│   │   └── docs/
├── README.md                    # Main project overview
└── prerequisites.md             # Global prerequisites for all labs
```
