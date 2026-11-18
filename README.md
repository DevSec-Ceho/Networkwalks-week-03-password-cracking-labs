 <div align="center">

# WEEK 03 – PASSWORD CRACKING LABS

### Cybersecurity & Ethical Hacking Practical Training

**NetworkWalks | Week 03 | Project Modules 01 & 02**

<img src="https://img.shields.io/badge/Training-NetworkWalks-blue?style=for-the-badge" alt="NetworkWalks Training">
<img src="https://img.shields.io/badge/Week-03-blue?style=for-the-badge" alt="Week 03">
<img src="https://img.shields.io/badge/Focus-Password%20Cracking-red?style=for-the-badge" alt="Password Cracking">
<img src="https://img.shields.io/badge/Status-Completed-success?style=for-the-badge" alt="Completed">

</div>

---

## 📌 Project Overview

This repository documents my **Week 03 practical cybersecurity exercises** as part of my Cybersecurity & Ethical Hacking practical training with **NetworkWalks**.

The exercises focused on understanding password security, extracting password hashes from password-protected PDF documents, and recovering the original passwords using different password-cracking tools.

During this week's practical sessions, I completed two project modules, exploring both a desktop-based password-cracking approach and browser-based password-recovery tools.

The first module involved using **John the Ripper (JTR)** through its graphical interface, **Johnny GUI**, while the second module introduced me to the **NetworkWalks Hash Calculator and Password Cracker**.

Through these exercises, I gained practical experience in extracting PDF password hashes, preparing hash files, loading hashes into password-cracking tools, executing password-recovery processes, and verifying recovered passwords.

The primary objective was to understand how password recovery works in practice and recognize the security implications of weak and easily guessable passwords.

## 🎯 Project Objectives

The main objectives of these practical exercises were to:

- Understand the fundamentals of password cracking and password security.
- Learn how password hashes are extracted from encrypted PDF documents.
- Gain practical experience using John the Ripper (JTR).
- Understand how to use Johnny GUI for password recovery.
- Explore the NetworkWalks Hash Calculator and Password Cracker.
- Compare desktop-based and browser-based password-recovery approaches.
- Understand how password candidates are tested against extracted hashes.
- Verify recovered passwords by opening password-protected PDF documents.
- Recognize the importance of strong passwords and secure file protection.

---

# 🧪 PROJECT MODULE 01: PASSWORD CRACKING WITH JOHN THE RIPPER (JTR)

## 1. Introduction

For the first project module, I used **John the Ripper (JTR)** and its graphical interface, **Johnny GUI**, to recover the password of a protected PDF document.

John the Ripper is a widely used password security auditing and recovery tool capable of working with different password hash formats.

Johnny provides a graphical interface that makes it easier to interact with John the Ripper without relying entirely on command-line operations.

The practical exercise involved extracting the password hash from a protected PDF document, saving the extracted hash in a text file, importing it into Johnny GUI, and initiating the password-recovery process.

## 2. Tools and Technologies Used

- John the Ripper (JTR)
- Johnny GUI
- Kali Linux / Windows environment
- PDF Hash Extractor
- Notepad
- Web browser
- Password-protected PDF document

## 3. Methodology and Practical Implementation

### Step 1: Downloading and Installing John the Ripper

I obtained John the Ripper and Johnny GUI and configured the application on my system.

I installed Johnny and configured it to locate the `john.exe` executable from the John the Ripper installation directory.

This allowed Johnny GUI to communicate with the John the Ripper engine and perform password-recovery operations through its graphical interface.

### Step 2: Extracting the PDF Password Hash

I obtained the password-protected PDF document and used an online PDF hash extraction tool to extract its password hash.

The extraction process generated a hash representation of the PDF password, which could then be processed by John the Ripper.

The extracted hash was in PDF hash format, beginning with:

`$pdf$`

### Step 3: Preparing the Extracted Hash File

After extracting the hash, I copied the complete hash value into a text file using Notepad.

I saved the file with the following filename:

`hash1.txt`

This file contained the extracted PDF password hash required by John the Ripper for the password-recovery process.

### Step 4: Loading the Hash into Johnny GUI

After preparing the hash file, I launched Johnny GUI.

I selected the option to open a password file and imported the previously created `hash1.txt` file.

Johnny GUI loaded the extracted hash and prepared it for the password-cracking operation.

### Step 5: Starting the Password-Recovery Process

With the hash successfully loaded, I initiated a new password-cracking operation using Johnny GUI.

The application processed the extracted PDF hash and attempted to recover the original password using its password-cracking capabilities.

During this process, John the Ripper tested password candidates against the extracted hash until it identified a matching password.

### Step 6: Recovering and Verifying the Password

The password-recovery process completed successfully, and the original password was recovered.

**Recovered Password:**

`good-luck`

After recovering the password, I returned to the password-protected PDF document and entered the recovered password.

The document opened successfully, confirming that the recovered password was correct.

## 4. Project Module 01 Result

<details>
<summary><strong>View Password Recovery Result – Module 01</strong></summary>

**Tool Used:** John the Ripper through Johnny GUI

**Hash File:** `hash1.txt`

**Recovered Password:** `good-luck`

**Verification:** Successfully opened the password-protected PDF document.

**Final Result:** Successful password recovery and document verification.

</details>

---

# 🧪 PROJECT MODULE 02: PASSWORD CRACKING WITH NETWORKWALKS TOOLS

## 1. Introduction

For the second project module, I explored an alternative approach to password recovery using two browser-based tools developed by **NetworkWalks**:

1. NetworkWalks Hash Calculator.
2. NetworkWalks Password Cracker.

Unlike the first module, which involved installing and configuring John the Ripper, this exercise demonstrated how password hashes can be extracted and processed using online tools.

The practical session involved uploading a protected PDF document to the NetworkWalks Hash Calculator, extracting its corresponding password hash, and submitting the extracted hash to the NetworkWalks Password Cracker.

The objective was to recover the original PDF password and verify the result by opening the protected document.

## 2. Tools and Technologies Used

- NetworkWalks Hash Calculator
- NetworkWalks Password Cracker
- Web browser
- Kali Linux / Windows environment
- Password-protected PDF document

## 3. Methodology and Practical Implementation

### Step 1: Obtaining the Password-Protected PDF

I downloaded the password-protected PDF document provided for the practical exercise.

The document required a password before its contents could be accessed.

### Step 2: Accessing the NetworkWalks Hash Calculator

I opened the NetworkWalks Hash Calculator through the following link:

**Tool:** [NetworkWalks Hash Calculator](https://networkwalks.com/hash-calculator/)

This tool was used to process the protected PDF document and extract its corresponding password hash.

### Step 3: Uploading the PDF and Extracting Its Hash

I uploaded the password-protected PDF document to the NetworkWalks Hash Calculator.

The tool processed the document and generated its corresponding PDF password hash.

This extracted hash served as the input for the next stage of the password-recovery process.

### Step 4: Copying the Extracted PDF Hash

After the hash extraction process was completed, I copied the complete hash value generated by the calculator.

I ensured that the entire hash was selected and copied correctly, including the portion beginning with:

`$pdf$`

The extracted hash was then prepared for submission to the password-cracking tool.

### Step 5: Accessing the NetworkWalks Password Cracker

Next, I opened the NetworkWalks Password Cracker using the following link:

**Tool:** [NetworkWalks Password Cracker](https://networkwalks.com/password-cracker/)

This tool was used to process the extracted PDF hash and perform the password-recovery operation.

### Step 6: Submitting the Extracted Hash

I pasted the previously extracted PDF password hash into the appropriate input field on the NetworkWalks Password Cracker.

After confirming that the hash had been entered correctly, I initiated the password-recovery process.

The tool attempted password candidates against the supplied hash to identify the matching password.

### Step 7: Recovering the Password

The password-recovery process completed successfully.

The tool identified the original password associated with the protected PDF document.

**Recovered Password:**

`password1`

### Step 8: Verifying the Recovered Password

To confirm that the password had been recovered correctly, I returned to the password-protected PDF document.

I entered the recovered password:

`password1`

The document opened successfully, confirming that the password-recovery process was successful.

## 4. Project Module 02 Result

<details>
<summary><strong>View Password Recovery Result – Module 02</strong></summary>

**Tools Used:** NetworkWalks Hash Calculator and NetworkWalks Password Cracker

**Hash Format:** PDF password hash (`$pdf$`)

**Recovered Password:** `password1`

**Verification:** Successfully opened the password-protected PDF document.

**Final Result:** Successful password recovery and document verification.

</details>

---

## 📊 Comparison of Both Project Modules

The two practical modules demonstrated different approaches to extracting PDF password hashes and recovering their corresponding passwords.

| Feature | Module 01 | Module 02 |
|---|---|---|
| Approach | Desktop-based | Browser-based |
| Hash Extraction | PDF Hash Extractor | NetworkWalks Hash Calculator |
| Cracking Tool | John the Ripper | NetworkWalks Password Cracker |
| Interface | Johnny GUI | Web interface |
| Hash Format | PDF Hash (`$pdf$`) | PDF Hash (`$pdf$`) |
| Recovered Password | `good-luck` | `password1` |
| Result | Successful | Successful |

## 🔍 Key Learning Outcomes

Through these two practical exercises, I gained hands-on experience and a better understanding of several important password-security concepts.

My key learning outcomes include:

- **Password Hash Extraction:** Understanding how password hashes can be extracted from password-protected PDF documents.
- **John the Ripper:** Gaining practical experience using John the Ripper for password recovery.
- **Johnny GUI Configuration:** Learning how to configure and operate Johnny GUI as a graphical interface for John the Ripper.
- **Hash File Preparation:** Understanding how extracted hashes are saved in text files and prepared for password-cracking tools.
- **Browser-Based Password Recovery:** Exploring the NetworkWalks Hash Calculator and Password Cracker.
- **Password Candidate Testing:** Understanding how password candidates are tested against extracted hashes.
- **Password Verification:** Learning the importance of verifying recovered passwords by accessing the original protected documents.
- **Password Security Awareness:** Recognizing how weak and predictable passwords can compromise document security.

## 🔐 Security Takeaways

These practical exercises reinforced several important password-security principles:

1. **Use Strong Passwords:** Avoid short, common, or easily predictable passwords that may be recovered through password-cracking techniques.

2. **Use Unique Passwords:** Avoid reusing the same password across different accounts, documents, and applications.

3. **Protect Sensitive Documents:** Apply strong password protection to confidential files and ensure that access is limited to authorized individuals.

4. **Understand Password Hashing:** Password hashes are used in security mechanisms, and their protection depends on the hashing algorithm and implementation.

5. **Perform Authorized Security Audits:** Password security assessments can help identify weak passwords and improve an organization's overall security posture.

6. **Avoid Predictable Password Patterns:** Passwords based on common words, simple combinations, or easily guessed patterns can increase the risk of unauthorized access.

---

## 🛠️ Technologies and Tools

<div align="center">

<img src="https://img.shields.io/badge/John%20the%20Ripper-Password%20Auditing-black?style=flat-square" alt="John the Ripper">
<img src="https://img.shields.io/badge/Johnny-GUI-blue?style=flat-square" alt="Johnny GUI">
<img src="https://img.shields.io/badge/NetworkWalks-Hash%20Calculator-orange?style=flat-square" alt="NetworkWalks Hash Calculator">
<img src="https://img.shields.io/badge/Password%20Cracking-Security-red?style=flat-square" alt="Password Cracking">
<img src="https://img.shields.io/badge/PDF-Hash%20Extraction-blue?style=flat-square" alt="PDF Hash Extraction">
<img src="https://img.shields.io/badge/Kali%20Linux-Environment-blue?style=flat-square" alt="Kali Linux">

</div>

---

# 📸 PRACTICAL DEMONSTRATION – SCREENSHOTS

This section contains the practical evidence from both project modules.

The screenshots are organized sequentially to demonstrate the tools used, hash extraction procedures, password-recovery operations, and successful document verification.

Each screenshot represents a stage of the practical implementation.

## Module 01: Password Cracking with John the Ripper (JTR)

### Screenshot 01 – John the Ripper / Johnny GUI Setup

This screenshot demonstrates the installation and configuration of John the Ripper and Johnny GUI.

<!-- UPLOAD SCREENSHOT 01 HERE -->

### Screenshot 02 – PDF Hash Extraction

This screenshot shows the extraction of the password hash from the protected PDF document.

<!-- UPLOAD SCREENSHOT 02 HERE -->

### Screenshot 03 – Saving the Extracted Hash

This screenshot demonstrates saving the extracted PDF password hash into the `hash1.txt` file using Notepad.

<!-- UPLOAD SCREENSHOT 03 HERE -->

### Screenshot 04 – Loading the Hash into Johnny GUI

This screenshot shows the process of importing the prepared hash file into Johnny GUI.

<!-- UPLOAD SCREENSHOT 04 HERE -->

### Screenshot 05 – Password Cracking Process

This screenshot demonstrates the password-recovery operation being performed through Johnny GUI.

<!-- UPLOAD SCREENSHOT 05 HERE -->

### Screenshot 06 – Successful Password Recovery and PDF Verification

This screenshot provides evidence of the successful recovery of the password `good-luck` and verification by opening the protected PDF document.

<!-- UPLOAD SCREENSHOT 06 HERE -->

---

## Module 02: Password Cracking with NetworkWalks Tools

### Screenshot 07 – Accessing the NetworkWalks Hash Calculator

This screenshot shows the NetworkWalks Hash Calculator interface used for the second practical exercise.

<!-- UPLOAD SCREENSHOT 07 HERE -->

### Screenshot 08 – Uploading the Protected PDF and Extracting Its Hash

This screenshot demonstrates uploading the password-protected PDF and generating its corresponding hash.

<!-- UPLOAD SCREENSHOT 08 HERE -->

### Screenshot 09 – Copying the Extracted PDF Hash

This screenshot shows the extracted PDF hash being copied for submission to the password-cracking tool.

<!-- UPLOAD SCREENSHOT 09 HERE -->

### Screenshot 10 – Submitting the Hash to the NetworkWalks Password Cracker

This screenshot demonstrates submitting the extracted hash to the NetworkWalks Password Cracker and initiating the recovery process.

<!-- UPLOAD SCREENSHOT 10 HERE -->

### Screenshot 11 – Successful Password Recovery

This screenshot provides evidence of the successful recovery of the password `password1`.

<!-- UPLOAD SCREENSHOT 11 HERE -->

### Screenshot 12 – Opening the Protected PDF with the Recovered Password

This screenshot demonstrates using the recovered password to unlock and access the protected PDF document.

<!-- UPLOAD SCREENSHOT 12 HERE -->

---

## 📚 References and Learning Resources

The following resources were used during the practical exercises and are useful for further learning:

- [John the Ripper – Official Website](https://www.openwall.com/john/)
- [Johnny GUI – Official Documentation](https://openwall.info/wiki/john/johnny)
- [NetworkWalks Hash Calculator](https://networkwalks.com/hash-calculator/)
- [NetworkWalks Password Cracker](https://networkwalks.com/password-cracker/)
- [NetworkWalks – Official Website](https://www.networkwalks.com/)

## ⚠️ Disclaimer

This repository documents practical cybersecurity training exercises conducted in an authorized educational environment.

All password-recovery activities were performed for educational purposes using provided lab documents.

The tools and techniques discussed in this repository should only be used on files, systems, and data that you own or have explicit permission to assess.

Unauthorized access to protected files or systems may violate applicable laws and regulations.

## 🙏 Acknowledgement

Special thanks to **NetworkWalks** and **Waqas Karim (CCIE)** for providing practical cybersecurity learning opportunities, technical guidance, and hands-on project exercises.

This week's practical activities have helped strengthen my understanding of password security, PDF hash extraction, password-cracking tools, and the importance of implementing strong password-protection mechanisms.

I look forward to building on these skills through continued hands-on practice and further exploration of cybersecurity concepts.

---

<div align="center">

## WEEK 03 – PROJECT COMPLETED ✅

**Continuous Learning | Hands-on Practice | Cybersecurity & Ethical Hacking**

**Training Platform: NetworkWalks**

</div>
