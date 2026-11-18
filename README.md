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
<img width="887" height="440" alt="cracking 1" src="https://github.com/user-attachments/assets/bce96f3d-ce65-49fc-a423-c30e6e80614e" />

<img width="1920" height="1080" alt="Screenshot (318)" src="https://github.com/user-attachments/assets/9389ee49-e5de-4966-9df9-b3fc7d1b9eff" />

<img width="1920" height="1080" alt="Screenshot (319)" src="https://github.com/user-attachments/assets/42d1d459-5284-47dd-8a23-b5ed2baa5be9" />
<img width="1920" height="1080" alt="Screenshot (320)" src="https://github.com/user-attachments/assets/da190b1f-e6ab-4fca-9fd7-b05563ce30ec" />
<img width="1920" height="1080" alt="Screenshot (321)" src="https://github.com/user-attachments/assets/f0fd2b92-f3a1-48e7-9e47-96e0a1a08e2d" />
<img width="1920" height="1080" alt="Screenshot (322)" src="https://github.com/user-attachments/assets/2eaf1f25-a2b4-4b21-865f-bdc07b5d8a0f" />


## Module 02: Password Cracking with NetworkWalks Tools

<img width="1920" height="1080" alt="Screenshot (323)" src="https://github.com/user-attachments/assets/eb39fee2-2428-4d42-9af5-4bf5d1f9e299" />
<img width="1920" height="1080" alt="Screenshot (324)" src="https://github.com/user-attachments/assets/1a89445a-b482-454d-a542-8d494dc3aee9" />
<img width="1920" height="1080" alt="Screenshot (325)" src="https://github.com/user-attachments/assets/727dbbb8-7694-4fdf-bb68-fc2787c7a736" />
<img width="1920" height="1080" alt="Screenshot (326)" src="https://github.com/user-attachments/assets/f27f64e2-a64b-456c-9326-f8e4150adf02" />
<img width="1920" height="1080" alt="Screenshot (327)" src="https://github.com/user-attachments/assets/9127d52e-5fb6-47a0-a29e-9c9ecec81d2b" />


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
