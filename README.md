# Wilson Marco Kundya

IT Support Specialist | System Administrator | Cybersecurity Scholar & Robotics Educator

 Dar es Salaam, Tanzania  
 Portfolio Website: [dudasafarisadventures-bot.github.io/GitHub-portfolio](https://dudasafarisadventures-bot.github.io/GitHub-portfolio)  
 Contact: Connect via GitHub

---

##  Professional Summary

Results-driven IT Support Specialist, Computer Technology Educator, and System Administrator with practical expertise in enterprise cloud infrastructure, Group Policy enforcement, and network security operations. Currently pursuing a Bachelor of Applied Science in Information Technology and System Administration at Ensign College (BYU-Pathway Worldwide). Actively developing core competencies in threat detection, digital forensics, GRC, security assessments, and embedded robotics systems using industry-standard tools.

---

## 🛠️ Technical Skills & Tools

###  Cybersecurity & Digital Forensics
![Wireshark](https://img.shields.io/badge/Wireshark-167DA5?style=for-the-badge&logo=Wireshark&logoColor=white)
![Metasploit](https://img.shields.io/badge/Metasploit-123456?style=for-the-badge&logo=linux&logoColor=white)
![Splunk](https://img.shields.io/badge/Splunk-000000?style=for-the-badge&logo=Splunk&logoColor=white)
![Burp Suite](https://img.shields.io/badge/Burp_Suite-FF6600?style=for-the-badge&logo=burpsuite&logoColor=white)
![Digital Forensics](https://img.shields.io/badge/Digital_Forensics-20B2AA?style=for-the-badge&logo=searx&logoColor=white)
![GRC](https://img.shields.io/badge/GRC_%26_Risk_Management-004088?style=for-the-badge&logo=securityscorecard&logoColor=white)

###  Systems Administration & Cloud
![Windows Server](https://img.shields.io/badge/Windows_Server_2022%2F2025-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![Active Directory](https://img.shields.io/badge/Active_Directory-002244?style=for-the-badge&logo=microsoft&logoColor=white)
![AWS EC2](https://img.shields.io/badge/AWS_EC2-FF9900?style=for-the-badge&logo=amazonaws&logoColor=white)
![Azure](https://img.shields.io/badge/Microsoft_Azure-0089D6?style=for-the-badge&logo=microsoftazure&logoColor=white)
![Intune](https://img.shields.io/badge/Microsoft_Intune-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu_Server-E95420?style=for-the-badge&logo=ubuntu&logoColor=white)

###  Robotics, Embedded Systems & Hardware
![Arduino](https://img.shields.io/badge/Arduino_Uno-00979D?style=for-the-badge&logo=arduino&logoColor=white)
![C++](https://img.shields.io/badge/C%2B%2B-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white)
![Tinkercad](https://img.shields.io/badge/Tinkercad_Simulator-FFF400?style=for-the-badge&logo=autodesk&logoColor=black)
![CCTV & Repair](https://img.shields.io/badge/Hardware_Repair_%26_CCTV-333333?style=for-the-badge&logo=opsgenie&logoColor=white)

---

##  Robotics Engineering Projects (Arduino & Embedded Systems)

### 1.  LED Blink — Introduction to Digital Output Control
* *Platform & Tools:* Tinkercad Simulator | Arduino Uno R3 | C++ (Arduino Framework)
* *Overview:* Programmed a digital output mechanism to control an LED indicator at 1-second interval cycles using pinMode(), digitalWrite(), and delay().
* *Key Achievements:*
  * Calculated current-limiting resistor values (220 Ohm) to prevent LED overcurrent damage.
  * Successfully verified continuous 1000ms timing loops within the Tinkercad simulation environment.
* *Result:* Established core foundation in microcontroller digital signaling and hardware circuit safety.

### 2.  Button-Controlled LED — Digital Input & Conditional Logic
* *Platform & Tools:* Tinkercad Simulator | Arduino Uno R3 | Push Button | C++
* *Overview:* Designed a real-time Human-Machine Interface (HMI) where user button interaction dynamically triggers conditional output states (if/else logic).
* *Key Achievements:*
  * Implemented digitalRead() functions on digital Pin 2 to detect HIGH (5V) and LOW (0V) signal transitions.
  * Constructed a pull-down resistor circuit topology ensuring noise-free digital input detection.
* *Result:* Achieved zero-latency input-driven LED actuation, demonstrating foundational interactive embedded controls.

### 3.  Button-Controlled Buzzer — Auditory Feedback System
* *Platform & Tools:* Tinkercad Simulator | Arduino Uno R3 | Piezo Buzzer | C++
* *Overview:* Developed an auditory signaling system using a piezo buzzer triggered by digital button input to emit controlled acoustic frequencies.
* *Key Achievements:*
  * Applied tone(pin, frequency) and noTone(pin) functions to generate clean 1000 Hz audio signals upon button presses.
  * Integrated multi-component input/output handling within a real-time looping structure.
* *Result:* Successfully deployed functional auditory user feedback for interactive hardware applications.

---

##  Key Enterprise SysAdmin & Security Projects

### 1.  Active Directory DS & GPO Enterprise Administration
* *Environment:* AWS EC2 Cloud Instance | Windows Server 2022
* *Overview:* Architected and validated an Active Directory Domain Controller within a cloud-hosted infrastructure.
* *Key Achievements:*
  * Provisioned delegated domain administrator accounts following strict Role-Based Access Control (RBAC) principles.
  * Designed Organizational Units (OUs) and configured SMB network shares with least-privilege permissions.
  * Authored and enforced domain-wide Group Policy Objects (GPOs) for centralized workstation customization and compliance.
* *Result:* Objectives fully verified on the live domain controller, demonstrating production-ready identity management skills.

### 2.  Automated Group Policy Folder Redirection
* *Environment:* Windows Server 2022 | Windows Client VM | GPMC
* *Overview:* Centralized user profile data and automated network backups by implementing Group Policy Folder Redirection.
* *Key Achievements:*
  * Established secure shared redirection roots with automated subfolder provisioning per domain user.
  * Enforced real-time policy updates using gpupdate /force and audited client compliance via gpresult /v.
* *Result:* Successfully migrated local user data to centralized storage, enhancing enterprise data resilience and security.

### 3.  Peer-to-Peer (P2P) Workgroup Cloud Architecture
* *Environment:* AWS EC2 Windows Server Instances | Advanced Sharing
* *Overview:* Configured a secure virtual P2P file-sharing network across isolated AWS cloud servers without relying on a full domain infrastructure.
* *Key Achievements:*
  * Implemented Advanced Sharing permissions and configured direct UNC paths (\\EC2AMAZ-CQRDC C5\Project5).
  * Resolved path-syntax challenges to ensure reliable network visibility and seamless resource sharing across workgroups.
* *Result:* Confirmed precise administrative control over network resource accessibility in cloud workgroup environments.

### 4.  User Account Security & Restriction Configuration
* *Environment:* Windows Server / Windows 11 | MMC Console
* *Overview:* Configured account lockout policies and system restrictions to enhance endpoint access security.
* *Key Achievements:*
  * Created a restricted user account (Project4) configured with a custom Microsoft Management Console (MMC).
  * Enforced strict Control Panel and system setting restrictions benchmarked against an unrestricted ClientAdmin administrator account.
* *Result:* Validated effective user privilege isolation and access controls across enterprise endpoints.

### 5.  Legacy Hardware Optimization: Windows 11 Pro Deployment
* *Environment:* Windows 11 Pro (25H2) | Unsupported Hardware | Local Utilities
* *Overview:* Resolved setup freeze points and successfully deployed Windows 11 Pro on legacy hardware failing official TPM 2.0 requirements.
* *Key Achievements:*
  * Diagnosed setup stalls during online update checks and bypassed network blocks using targeted local installation overrides.
  * Successfully completed first-time setup while maintaining complete integrity of user files, system configurations, and software suites.
* *Result:* Extended the operational lifecycle of legacy hardware without compromising system stability or data integrity.

---

##  Professional Experience

###  St. Columba's English Medium Primary School | Dar es Salaam, Tanzania
*Computer Technology Teacher & IT Support Specialist* (Jan 2025 – Present)
* Teach foundational and modern technology courses including *Computer Basics, Artificial Intelligence (AI) Basics, and Basic Robotics* to primary school students using hands-on methodologies.
* Manage and maintain school-wide computer laboratory infrastructure, serving as the primary IT Help Desk support for resolving hardware, software, and network connectivity issues.
* Implement technology-integrated learning, device setup, and endpoint maintenance across administrative and academic workstations.

###  3113Tech Solutions | Dar es Salaam, Tanzania
*Founder & Lead IT Consultant* (Present)
* Deliver end-to-end IT support, network deployments, and CCTV security installations for enterprise clients.
* Administer Windows Server environments, remote assistance setups, and custom IT infrastructure projects.

---

##  Certifications & Academic Background

###  Academic Degrees & BYU-Pathway Credentials
*  *B.A.S. in Information Technology & System Administration (Cybersecurity Focus)*  
  Ensign College / BYU-Pathway Worldwide | Expected Graduation: Sept 2027
*  *PathwayConnect Certificate* – BYU-Pathway Worldwide | *Completed March 2026*
*  *Self-Reliance Certificate* – BYU-Pathway Worldwide | *Completed 2026*
*  *Diploma in Education* – Bunda Teachers Training College
*  *A-Level Certificate* – Mwenge High School (2007)
*  *O-Level Certificate* – Ihanja Technical School (1999)

###  Industry Certifications & Training Paths
*  *CompTIA Security+ (SY0-701)* – In Progress (uCertify Exam Prep)
*  *CS50: Introduction to Cybersecurity* – Harvard University / edX (In Progress)
*  *TryHackMe:* Pre-Security & SOC Level 1 Learning Paths – In Progress
*  *Cisco Networking Academy:* Network Support & Security; Network Technician (2026)
*  *Cisco Networking Academy:* Splunk Cybersecurity Defense Analyst Journey

###  Completed Professional Certificates (October 2026)
* *Learning Cyber Incident Response & Digital Forensics* (LinkedIn Learning)
* *Performing a Technical Security Assessment* (LinkedIn Learning)
* *AI for GRC Analysts* (by Cybrary) (LinkedIn Learning)
* *CompTIA A+ Core 1 (220-1101) Prep* (LinkedIn Learning)
* *Introduction to Artificial Intelligence* (LinkedIn Learning)
* *Computer Science Principles: Digital Information* (LinkedIn Learning)
* *Teaching with Technology* (LinkedIn Learning)
* *Teamwork Foundations* (LinkedIn Learning)

---

##  Core Strengths & Value-Add Capabilities

*  *Technical Troubleshooting & Root Cause Analysis:* Proficient in diagnosing complex hardware, operating system, and network connectivity faults quickly to reduce system downtime.
*  *Security-First Mindset:* Combining system administration experience with SOC and digital forensics methodologies to enforce Zero Trust access control and identity governance.
*  *Robotics & STEM Education Leadership:* Expertise in simplifying complex engineering topics (Arduino, C++, circuit design, AI basics) to educate and inspire students.
*  *Versatility & Rapid Adaptability:* Proven track record of continuously expanding technical skillsets across cloud infrastructure (AWS/Azure), enterprise systems (Windows Server/Active Directory), and modern AI security applications.

---

###  Let's Connect & Collaborate!

I am actively seeking opportunities as a Security Analyst I, SOC Analyst, System Administrator, or STEM/Robotics Instructor*.  
Feel free to reach out for consultations, technical collaborations, or professional opportunities!

[ Send an Email](mailto:wilsonmichael0014@gmail.com) | [ Chat on WhatsApp](https://wa.me/2557400221000) | [ Visit Personal Website](https://www.wilson-marco.org)

