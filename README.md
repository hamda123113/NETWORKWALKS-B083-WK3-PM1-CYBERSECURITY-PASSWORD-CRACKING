# NETWORKWALKS-B082-WK3-PM1-CYBERSECURITY-PASSWORD-CRACKING
<div align="center">

# 🔐 Password Cracking with John the Ripper

**Recovering the password of a protected PDF using JTR John and JTR Johnny in a controlled cybersecurity lab**

</div>

<p align="center">
  <img src="https://img.shields.io/badge/Skill-Cybersecurity-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Project-Password%20Cracking-C00000?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Tool-John%20the%20Ripper-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/GUI-Johnny-404040?style=flat-square&labelColor=0070C0" />
  <img src="https://img.shields.io/badge/OS-Kali%20Linux-404040?style=flat-square&labelColor=C00000&logo=kalilinux&logoColor=white" />
  <img src="https://img.shields.io/badge/Target-Protected%20PDF-E87500?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/Skill-Linux-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Skill-Ethical%20Hacking-404040?style=flat-square&labelColor=C00000" />
  <img src="https://img.shields.io/badge/Virtualization-VirtualBox-0070C0?style=flat-square&labelColor=000000" />
  <img src="https://img.shields.io/badge/GitHub-404040?style=flat-square&labelColor=0070C0&logo=github&logoColor=white" />
  <img src="https://img.shields.io/badge/NetworkWalks-404040?style=flat-square&labelColor=C00000" />
</p>

---

## 📌 Project Overview

This project demonstrates how **John the Ripper (JTR)** and its graphical interface **Johnny** can be used in a controlled cybersecurity laboratory to recover the password of a protected PDF file.

The practical was performed using a Kali Linux virtual machine and a test PDF supplied for the exercise.

The workflow includes:

- Preparing the JTR/Johnny environment
- Obtaining the protected PDF
- Extracting the PDF password hash
- Saving the hash into a text file
- Importing the hash into Johnny
- Starting a password-recovery attack
- Recovering the password
- Using the recovered password to open the protected PDF

John the Ripper is commonly used by security professionals for password-strength testing and supports multiple password-hash formats and protected file types. :contentReference[oaicite:2]{index=2}

---

## 🎯 Objectives

The main objectives of this project are to:

- Understand the basic concept of password cracking.
- Install/use **John the Ripper**.
- Use **Johnny GUI** to interact with JTR.
- Obtain the hash representation of a protected PDF.
- Save the extracted hash into a `.txt` file.
- Import the hash into Johnny.
- Start a controlled password-recovery attack.
- Recover the password of the provided test PDF.
- Verify the recovered password by opening the PDF.
- Document the complete cybersecurity workflow.

---

## 🛡️ Purpose of the Lab

This project is intended for **educational and authorized cybersecurity testing**.

Password-cracking tools can be used to evaluate password security, but they should only be used against files, accounts, systems, or environments that you own or have explicit permission to test.

⚠️ **Important:** Do not use John the Ripper or similar tools to access unauthorized accounts, files, systems, or services.

---

# 🏗️ Lab Environment

The practical was performed inside a virtualized Kali Linux environment.

### Lab Architecture

```text
┌─────────────────────────────┐
│       Host Computer         │
│                             │
│      Windows / Host OS      │
└──────────────┬──────────────┘
               │
               │ VirtualBox
               ▼
┌─────────────────────────────┐
│       Kali Linux VM         │
│                             │
│  ┌───────────────────────┐  │
│  │ John the Ripper (JTR) │  │
│  └───────────────────────┘  │
│              │              │
│              ▼              │
│       ┌─────────────┐       │
│       │   Johnny    │       │
│       │     GUI     │       │
│       └──────┬──────┘       │
│              │              │
│              ▼              │
│       PDF Password Hash     │
│              │              │
│              ▼              │
│       Password Recovery     │
└─────────────────────────────┘
