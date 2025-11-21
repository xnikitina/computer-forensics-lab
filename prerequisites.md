# Prerequisites for Lab Environment

This document outlines the system requirements and forensic tools needed to complete the lab exercises.  
All tools must be installed locally on your Windows environment before starting the labs.

---

## 🖥️ System Requirements

- **Operating Systems**
  - Windows 11 (Virtual Machine or physical)

- **Virtualization Software (Optional)**
  - VirtualBox or VMware Workstation (recommended for isolated lab environments)

- **Network**
  - Stable internet connection for tool downloads and updates

- **Permissions**
  - Administrator privileges required to install and run forensic tools

---

## 🧰 Required Forensic Tools (Local Installation)

The following tools are required for the six core lab exercises.  
Download and install them from their official sources:

| Tool                          | Purpose                                               | Official Download Link |
|-------------------------------|-------------------------------------------------------|------------------------|
| **File Viewer Lite**          | View files in various formats (e.g., .doc, .pdf, .jpg)| [File Viewer Lite](https://fileviewer.com/lite/) |
| **R-Drive Image**             | Create disk image files of hard disk partitions       | [R-Drive Image](https://www.r-tt.com/Download/RDriveImageDownload.shtml) |
| **EaseUS Data Recovery Wizard** | Recover deleted files from evidence sources         | [EaseUS Data Recovery Wizard](https://www.easeus.com/datarecoverywizardpro/) |
| **FTK Imager**                | Disk imaging, file extraction, and evidence preview   | [FTK Imager](https://accessdata.com/product-download/ftk-imager) |
| **HashCalc**                  | Generate hash values (MD5, SHA-1, SHA-256)            | [HashCalc](https://www.slavasoft.com/hashcalc/) |
| **MD5 Calculator**            | Calculate MD5 checksums for integrity verification    | [MD5 Calculator](https://www.softpedia.com/get/Security/Encrypting/MD5-Calculator.shtml) |

---

## 🔧 Additional Development & Network Tools

These tools are required to support lab exercises involving scripting, network analysis, and compliance testing.  
Download and install them from their official sources:

| Tool/Folder Name               | Purpose / Role                          | Required Installer File(s) | Official Download Link |
|--------------------------------|------------------------------------------|----------------------------|------------------------|
| **Adobe Reader**               | PDF viewer for documentation             | —                          | [Adobe Reader](https://get.adobe.com/reader/) |
| **Java Runtime Environment (JRE 8u391)** | Java application runtime | `jre-8u391-windows-x64.exe` | [Java Runtime Environment 8u391](https://www.java.com/en/download/manual.jsp) |
| **Java SE Development Kit (JDK 21)**  | Java development and compilation | `jdk-21_windows-x64_bin.exe` | [Java SE Development Kit 21](https://www.oracle.com/java/technologies/downloads/) |
| **Microsoft Visual C++ Redistributables** | Runtime libraries for C++ applications (required for legacy and modern tools) | `vcredist_2010_sp1_x64.exe`<br>`vcredist_2010_sp1_x86.exe`<br>`vcredist_2012_upd4_x64.exe`<br>`vcredist_2012_upd4_x86.exe`<br>`vcredist_2013_upd5_x64.exe`<br>`vcredist_2013_upd5_x86.exe`<br>`vcredist_2022_x64.exe`<br>`vcredist_2022_x86.exe` | [Visual C++ Redistributables](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170) |
| **Notepad++**                  | Editor for scripts and logs              | `npp.8.5.8.Installer.x64.exe` | [Notepad++](https://notepad-plus-plus.org/downloads/) |
| **PuTTY**                      | SSH/Telnet client                        | `putty-64bit-0.79-installer.msi` | [PuTTY](https://www.putty.org/) |
| **WampServer**                 | Local web server (Apache, MySQL, PHP)    | `wampserver3.3.0_x64.exe` | [WampServer](https://www.wampserver.com/en/download-wampserver-64bits/) |
| **Web Browsers (Chrome, Firefox, Edge)** | UI validation and cross-browser testing | `ChromeSetup.exe`<br>`Firefox Installer.exe` | [Chrome](https://www.google.com/chrome/), [Firefox](https://www.mozilla.org/firefox/), [Edge](https://www.microsoft.com/edge) |
| **WinPcap**                    | Network traffic capture library          | `WinPcap_4_1_3.exe` | [WinPcap](https://www.winpcap.org/install/) |
| **WinRAR**                     | File compression and archiving           | `winrar-x64-624.exe` | [WinRAR](https://www.win-rar.com/download.html) |

---

## 🛠️ Visual C++ Redistributable Verification Script (PowerShell)

Use the following PowerShell script to verify that all required Visual C++ Redistributables are installed:

```powershell
$requiredVersions = @(
    "Microsoft Visual C++ 2010  x64 Redistributable - 10.0.40219",
    "Microsoft Visual C++ 2010  x86 Redistributable - 10.0.40219",
    "Microsoft Visual C++ 2012 x64 Additional Runtime - 11.0.61030",
    "Microsoft Visual C++ 2012 x86 Additional Runtime - 11.0.61030",
    "Microsoft Visual C++ 2013 x64 Additional Runtime - 12.0.40664",
    "Microsoft Visual C++ 2013 x86 Additional Runtime - 12.0.40664",
    "Microsoft Visual C++ 2022 X64 Additional Runtime",
    "Microsoft Visual C++ 2022 X86 Additional Runtime"
)

$installed = Get-WmiObject -Class Win32_Product | Select-Object -ExpandProperty Name
foreach ($version in $requiredVersions) {
    if ($installed -contains $version) {
        Write-Host "$version is installed." -ForegroundColor Green
    } else {
        Write-Host "$version is NOT installed." -ForegroundColor Red
    }
}
