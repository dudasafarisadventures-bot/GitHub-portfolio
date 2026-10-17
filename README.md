# Wilson Marco Kundya
IT Support | Cybersecurity Student | 3113Tech Solutions

### Education
Bachelor of Applied Science, Information Technology and System Administration (Cybersecurity Focus)
Ensign College – BYU-Pathway Worldwide | Expected September 2027

### Work Experience
**IT Support & Computer Technology Teacher @ St. Columba's School, Dar es Salaam**
- Manage IT support for the school
- Teach Computer Technology to O-Level students

**Founder @ 3113Tech Solutions**
- IT support and CCTV installation services

## Projects

### IT312 – Vulnerability Assessment & Mitigation
**Ensign College – BYU-Pathway Worldwide** | Cybersecurity Foundations

**Overview:** Performed an Nmap SYN Stealth scan with service/version detection against a Metasploitable host in a controlled Cyber Range lab. Identified 23 open TCP services out of 1000 scanned, then assessed risk and wrote mitigation recommendations following Blue Team best practices.

**Tools:** Nmap, Metasploitable, Cyber Range lab

**Key Findings:**

| Port / Service | Vulnerability | Risk |
|---|---|---|
| 1524/tcp (bindshell) | Unauthenticated root shell | Critical |
| 21/tcp (vsftpd 2.3.4) | Known backdoor | Critical |
| 23/tcp (Telnet) | Unencrypted authentication | High |
| 512-514/tcp (r-services) | Insecure legacy remote access | High |
| 80/tcp (Apache 2.2.8) | Outdated web server | Medium |
| 139/445/tcp (Samba 3.x) | Outdated SMB implementation | Medium |
| 2049/tcp (NFS) | Potential misconfigured file access | Medium |
| 22/tcp (OpenSSH 4.7p1) | Outdated SSH version | Low |

**Result:** Scan completed in about 12 seconds. Delivered an executive summary with risk ratings and mitigation steps.

---

### IT312 – Project #7: TechLab Network Reconnaissance
**Ensign College – BYU-Pathway Worldwide** | Cybersecurity Foundations | July 2026

**Overview:** Acting as a newly hired penetration tester, I performed the first step of the Cyber Kill Chain (target reconnaissance) against the TechLab network. The goal was to find live hosts, identify which expose the largest attack surface, and select five priority targets for a follow-on engagement.

**Tools:** Nmap 7.95, Kali Linux VM, Terminal

**What I did:**
- Calculated the subnet range (172.29.16.0/20, 4,096 addresses) from my own VM address
- Ran a full-subnet discovery scan, saved as evidence with `-oN`
- Found ICMP was being filtered, so I switched to TCP SYN probes and discovered **95 live hosts**
- Reviewed open ports and services on each host

**Five priority targets selected:**

| Host | Why selected |
|---|---|
| Linux (Metasploitable) | 14 open ports, outdated UnrealIRCd 3.2.8.1 with a known backdoor |
| Linux (cloned build) | Identical services to the first host, so one exploit works on both |
| Windows host | RDP (3389) exposed, common entry for brute-force attacks |
| Windows host | Second RDP target, higher chance of weak or reused credentials |
| DNS server (Unbound) | Strategic target: compromising DNS can redirect traffic for the whole subnet |

**Result:** Mapped a /20 subnet and prioritized targets by attack surface, service age and strategic value, as a real penetration tester would.

---

### IT312 – SSH Brute Force Attack using Metasploit Framework
**Ensign College – BYU-Pathway Worldwide** | Cybersecurity Foundations

**Overview:** Conducted a successful SSH brute force attack against a deliberately vulnerable Metasploitable server, using the Metasploit Framework, to demonstrate offensive security methodology and the risk of weak default credentials.

**Tools:** Metasploit Framework, Metasploitable (isolated lab VM)

**What I did:**
- Selected the `auxiliary(scanner/ssh/ssh_login)` module to test SSH credentials
- Configured the target with `set RHOSTS`
- Set default credentials (`msfadmin` / `msfadmin`) known to be weak on Metasploitable
- Ran the attack with `run` and confirmed successful authentication

**Result:** ✅ Successfully authenticated via SSH using default credentials, demonstrating how unchanged default logins create a critical attack vector, and why credential management and access control matter.

---

### Windows Server Active Directory Domain Controller – Configuration & Group Policy Management
**Ensign College – BYU-Pathway Worldwide** | IT125 – Introduction to Information Technology | AWS EC2 (Windows Server)

**Overview:** Deployed and configured a Windows Server Active Directory Domain Controller in a cloud-hosted lab on AWS EC2, simulating the responsibilities of a Windows systems administrator managing a small-to-medium enterprise domain.

**Tools:** AWS EC2, Active Directory Domain Services (AD DS), Server Manager, Active Directory Users and Computers, Group Policy Management Console (GPMC)

**What I did:**
- Reviewed the domain controller's baseline configuration via Server Manager
- Created a delegated administrator account and granted it Domain Admins rights
- Created and later deleted an Organizational Unit (OU), including disabling the "Protect object from accidental deletion" safeguard
- Configured an SMB network share with least-privilege (read-only) access
- Authored a domain-wide Group Policy Object (GPO) to centrally enforce a desktop wallpaper across all domain workstations
- Validated policy deployment with a live sign-out/sign-in test on the domain controller

**Key Skills Demonstrated:**
- Active Directory Domain Services (AD DS) administration
- Role-based account provisioning (Domain Admins delegation)
- OU design and Group Policy inheritance principles
- SMB file sharing and NTFS/share-level permissions
- GPO authoring and deployment via GPMC
- Cloud-hosted Windows Server administration on AWS EC2
- Remote systems management via RDP and AWS Fleet Manager

**Result:** All objectives independently verified end-to-end — account provisioning, OU lifecycle, network share, and GPO enforcement confirmed by direct observation on the domain controller.

---

### Remote Access Technologies – Remote Desktop Connection & File Transfer
**Ensign College – BYU-Pathway Worldwide** | PC103 | April 2026

**Overview:** Set up and tested remote access between two laptops on the same network, demonstrating how to remotely view/control a device and transfer files securely — a core IT support and help desk skill.

**Tools:** AnyViewer (remote access software)

**What I did:**
- Installed AnyViewer on both laptops and signed in with separate accounts
- Established a remote connection using device ID and login credentials
- Remotely navigated files and opened applications on the connected laptop
- Used the file transfer feature to send and confirm receipt of documents between devices
- Documented the process with screenshots as evidence
- Closed the session safely after completing all tasks

**Challenges & Resolutions:**
- Internet speed occasionally affected connection performance
- Initial setup required careful account/login management across two separate accounts
- Minor file-transfer delays were resolved by confirming receipt on both ends

**Result:** Successfully connected two laptops, remotely controlled one device from the other, and transferred files end-to-end — confirming reliable remote access setup and operation.

---

### Installing Windows 11 on Unsupported Hardware
**Personal / Practical IT Support Project** | July 2026 | Dar es Salaam, Tanzania

**Overview:** Upgraded a personal laptop to Windows 11 Pro despite it not meeting Microsoft's official hardware requirements (e.g., TPM 2.0). Setup initially froze during the update-checking phase; this documents the diagnosis and the fix that led to a successful install.

**Tools:** Windows 11 installation media, local laptop hardware

**Problem:** Setup froze at 46% on "Checking for updates," unresponsive for 25+ minutes due to an unstable connection to Microsoft's update servers.

**What I did:**
- Disabled Wi-Fi to force Setup to stop waiting on the update server, confirmed it was still frozen
- Performed a forced shutdown and manual restart, then relaunched `setup.exe` directly
- On relaunch, selected **"Not right now"** instead of "Download updates, drivers and optional features" to skip the online update check entirely
- Accepted the hardware compatibility warning, knowingly proceeding on unsupported hardware
- Chose Install: Windows 11 Pro, keeping personal files and apps
- Monitored installation through to 100% without stalling, then completed first-time setup

**Result:** Windows 11 Pro (25H2) installed successfully with all personal files, folders, and previously installed applications (Chrome, Opera, VLC, Avast One, Arduino IDE, etc.) preserved intact.

**Key lesson:** Windows 11 can be installed on unsupported hardware once the compatibility warning is accepted, and skipping the online update check during Setup is an effective way to avoid a common freeze point caused by unstable internet.

---

### Peer-to-Peer Workgroup File Sharing on AWS Windows Server
**Dar es Salaam, Tanzania** | Networking Project

**Overview:** Configured a virtual Peer-to-Peer (P2P) file-sharing network on an AWS Windows Server instance, establishing secure directory sharing and network visibility without a full domain architecture.

**Tools:** AWS Windows Server (EC2), Windows Advanced Sharing, Windows Run utility

**Problem:** Isolated cloud servers lacked a collaborative framework for sharing files across a workgroup without setting up a complex domain.

**What I did:**
- Created a designated shared folder (`C:\Project5`) and enabled Advanced Sharing
- Granted full permissions to the "Everyone" group for workgroup-level access
- Resolved a minor path-syntax issue during setup
- Verified connectivity and access using the Windows Run utility and the resulting network path (`\\EC2AMAZ-CQRDCC5\Project5`)
- Captured evidence of sharing settings, permissions, and successful peer-to-peer access

**Result:** Successfully proved administrative control over resource accessibility — confirming that correct permission management and precise network paths are what make peer-to-peer file sharing work reliably.

---

### Project #11 – Group Policy Folder Redirection
**Ensign College – BYU-Pathway Worldwide** | Windows Server Administration

**Overview:** Configured Group Policy Folder Redirection on a Windows Server 2022 Domain Controller, redirecting users' Documents folder from local storage to a shared network location — a common enterprise technique for centralizing and backing up user data.

**Tools:** Windows Server 2022, Active Directory Users and Computers, Group Policy Management Console (GPMC), Windows Client VM

**What I did:**
- Created a shared "Redirection" folder on the Domain Controller with Read/Write access for Everyone
- Created and linked a new GPO ("Folder Redirection") to the domain
- Configured Basic folder redirection for the Documents folder, with a dedicated subfolder per user under the shared root path
- Set the policy to redirect folders back to the local user profile if the policy is ever removed
- Applied the policy with `gpupdate /force` and verified it client-side with `gpresult /v`
- Confirmed via File Explorer that the Documents folder — and the files inside it — now pointed to the server location instead of the local drive

**Result:** Successfully redirected user Documents folders to centralized network storage, confirmed end-to-end by checking folder properties and file locations after policy application.

## Contact
Portfolio: [wilson-marco.org](https://wilson-marco.org)
