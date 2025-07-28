# Fundamentals of Information Security - Lab Solutions

This repository contains complete solutions for the Fundamentals of Information Security course lab assignments. Each lab focuses on different aspects of cybersecurity, providing hands-on experience with essential security tools and techniques.

## 📚 Course Overview

This repository documents practical implementations and solutions for six comprehensive laboratories covering:

- Cryptography and Steganography
- Web Application Security  
- Malware Analysis
- Operating System Security & Penetration Testing
- Software Security & Buffer Overflow
- Digital Forensics

## 🗂️ Repository Structure

```log
├── README.md
├── Lab01/          # Crypto Basics
├── Lab02/          # Web Application Security
├── Lab03/          # Malware Analysis
├── Lab04/          # OS Security & Penetration Testing
├── Lab05/          # Software Security & Buffer Overflow
└── Lab06/          # Digital Forensics
```

## 🔬 Lab Details

### Lab 01 - Crypto Basics

**Topics:** Cryptography Algorithms, Steganography

- Implementation of substitution cipher encryption/decryption
- Steganography techniques (video, audio, ICMP/DNS)
- RSA key generation and digital signatures
- Caesar cipher decoding

**Key Files:**

- [`Lab01/lab1_solution.md`](Lab01/lab1_solution.md) - Complete solutions with screenshots
- [`Lab01/videostego/`](Lab01/videostego/) - Video steganography tools
- [`Lab01/code/`](Lab01/code/) - Cryptography implementations

### Lab 02 - Web Application Security

**Topics:** Web vulnerabilities, Authentication, OWASP Top 10

- Flask web application development with database connectivity
- Authentication mechanisms (Basic, Digest, Certificate)
- SQL injection prevention
- Network firewall configuration
- Password hashing and salting techniques

**Key Files:**

- [`Lab02/Lab02_solution.md`](Lab02/Lab02_solution.md) - Comprehensive security implementations
- [`Lab02/my_flask_app/`](Lab02/my_flask_app/) - Secure web application code

### Lab 03 - Malware Analysis

**Topics:** Dynamic Analysis, Sandbox Analysis, Incident Response

- Malware sandbox analysis using Any.run platform
- Dynamic behavior analysis and artifact identification
- Network traffic analysis and IOC extraction
- Remediation strategies and firewall rules

**Key Files:**

- [`Lab03/Lab03_solution.md`](Lab03/Lab03_solution.md) - Complete malware analysis report
- [`Lab03/malware_analysis_report_template.pdf`](Lab03/malware_analysis_report_template.pdf) - Professional reporting template

### Lab 04 - OS Security & Penetration Testing

**Topics:** Vulnerability Assessment, Metasploit Framework, Network Security

- Metasploitable 3 setup and configuration
- Vulnerability scanning with Nessus Essentials
- Exploitation using Metasploit Framework
- Persistence techniques and privilege escalation

**Key Files:**

- [`Lab04/Lab04_solution.md`](Lab04/Lab04_solution.md) - Penetration testing methodology
- [`Lab04/Metasploitable3-ub1404_9shq4j.pdf`](Lab04/Metasploitable3-ub1404_9shq4j.pdf) - Target environment documentation

### Lab 05 - Software Security & Buffer Overflow

**Topics:** Buffer Overflow Attacks, Memory Management, Exploitation Techniques

- Buffer overflow vulnerability analysis
- Stack-based buffer overflow exploitation
- Return Oriented Programming (ROP)
- Memory debugging with Valgrind
- Segmentation fault analysis and prevention

**Key Files:**

- [`Lab05/Lab_5_Buffer_overflow.html`](Lab05/Lab_5_Buffer_overflow.html) - Lab instructions and methodology

### Lab 06 - Digital Forensics

**Topics:** Forensic Imaging, Evidence Integrity, Timeline Analysis

- CAINE Linux forensic environment setup
- Forensic disk imaging using Guymager
- Hash verification and chain of custody procedures
- Timeline analysis and artifact recovery
- Technical analysis using Autopsy

**Key Files:**

- [`Lab06/Lab06_solution.md`](Lab06/Lab06_solution.md) - Complete forensic investigation
- [`Lab06/screenshots/`](Lab06/screenshots/) - Evidence documentation

## 🛠️ Tools & Technologies Used

### Cryptography & Security Tools

- OpenSSL for RSA key management
- Steghide for audio steganography
- Custom cipher implementations

### Web Security

- Flask framework with SQLite
- UFW firewall configuration
- SHA-256 hashing with salt

### Malware Analysis

- Any.run sandbox platform
- Network traffic analysis tools
- IOC extraction and analysis

### Penetration Testing

- Kali Linux penetration testing distribution
- Metasploit Framework
- Nessus vulnerability scanner
- Nmap network discovery

### Software Security

- Buffer overflow analysis tools
- Valgrind memory debugging
- GDB debugging environment
- Return Oriented Programming techniques

### Digital Forensics

- CAINE Linux forensic distribution
- Guymager disk imaging tool
- Autopsy forensic analysis platform
- Timeline analysis tools (log2timeline.py)

## 📖 Learning Outcomes

Upon completion of these labs, students will have practical experience with:

- **Cryptographic Operations:** Implementing ciphers, managing keys, digital signatures
- **Web Security:** Identifying vulnerabilities, implementing secure authentication
- **Malware Analysis:** Dynamic analysis techniques, threat intelligence gathering
- **Penetration Testing:** Vulnerability assessment, exploitation techniques
- **Software Security:** Buffer overflow analysis, memory exploitation, secure coding
- **Digital Forensics:** Evidence acquisition, integrity verification, timeline analysis

## 📝 Documentation

Each lab includes:

- Detailed solution methodology
- Step-by-step implementation guides
- Screenshots and evidence documentation
- Code implementations and scripts
- Professional reporting templates

## 👥 Contributors

- **Mohamad Nour Shahin** - Primary contributor
- **Anas Atasi** - Lab 06 contributor  
- **Hayder Sarhan** - Lab 06 contributor

**Group:** B22-CBS-01

---
