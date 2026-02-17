# 🔴 Advanced Red Teaming Roadmap & Resources

[![Learning](https://img.shields.io/badge/Learning-RedTeam-blue?style=flat-square)](https://www.hackthebox.com/) [![Skills](https://img.shields.io/badge/Skills-Advanced-yellow?style=flat-square)]() [![Labs](https://img.shields.io/badge/Labs-Practice-green?style=flat-square)]()

> This repository provides a structured **Advanced Red Teaming Roadmap** along with curated learning resources, tools, and labs to help you master real-world adversary emulation.

---

## 🎯 Roadmap Overview

| Phase | Focus Area | Key Skills | Resources / Tools |
|-------|------------|------------|-----------------|
| 0 | Foundations | Networking, OS Internals, Programming | [Practical Networking](https://www.practicalnetworking.net/), [Windows Internals](https://learn.microsoft.com/en-us/sysinternals/resources/windows-internals) |
| 1 | Exploit Development | Buffer Overflow, Heap, Shellcode | [Exploit Education](https://exploit.education/), [Pwn College](https://pwn.college/) |
| 2 | Active Directory | Kerberoasting, DCSync, Golden/Silver Ticket | [BloodHound](https://github.com/BloodHoundAD/BloodHound), [Rubeus](https://github.com/GhostPack/Rubeus), [Impacket](https://github.com/fortra/impacket) |
| 3 | Evasion & Malware Dev | Process Hollowing, AMSI/EDR Bypass, C2 | [IredTeam](https://www.ired.team/), [Awesome Red Team](https://github.com/S3cur3Th1sSh1t/Awesome-Red-Team) |
| 4 | Command & Control (C2) | Beacon customization, Traffic shaping | [Sliver](https://github.com/BishopFox/sliver), [Havoc](https://github.com/HavocFramework/Havoc) |
| 5 | Adversary Emulation | MITRE ATT&CK mapping, Threat Intelligence | [MITRE ATT&CK](https://attack.mitre.org/), [Mandiant Resources](https://www.mandiant.com/resources) |
| 6 | Cloud Red Teaming | AWS & Azure attacks | [Hacking The Cloud](https://hackingthe.cloud/), [AWS IAM Escalation](https://github.com/RhinoSecurityLabs/AWS-IAM-Privilege-Escalation), [MicroBurst](https://github.com/NetSPI/MicroBurst) |
| 7 | Initial Access & Social Engineering | Phishing, Payload Obfuscation | [Evilginx2](https://github.com/kgretzky/evilginx2), [SET](https://github.com/trustedsec/social-engineer-toolkit) |

---

## 🧰 Recommended Tools

- **Red Teaming:** Cobalt Strike, Sliver, Havoc  
- **Active Directory:** BloodHound, Rubeus, Impacket, CrackMapExec  
- **Exploitation:** Metasploit, Immunity Debugger, GDB, pwntools  
- **Phishing & Social Engineering:** Evilginx2, Social Engineer Toolkit  
- **Cloud Pentesting:** AWS CLI, Azure AD, MicroBurst scripts  

---

## 🧪 Labs & Practice Platforms

| Platform | Description | Link |
|----------|------------|------|
| Hack The Box | Realistic VMs for pentesting & AD labs | https://www.hackthebox.com/ |
| TryHackMe | Guided rooms for beginner → advanced | https://tryhackme.com/ |
| Exploit Education | Exploit dev practice VMs | https://exploit.education/ |
| Pwn College | Exploit development & memory | https://pwn.college/ |
| PortsWigger Labs | Web security & phishing | https://portswigger.net/web-security |

---

## 📚 Books & References

- **Windows Internals, 7th Edition** – Mark Russinovich  
- **The Art of Memory Forensics** – Michael Hale Ligh  
- **The Shellcoder’s Handbook** – Chris Anley  
- SpecterOps Blog – https://posts.specterops.io/  
- Harmj0y Blog – https://blog.harmj0y.net/  

---

## 🏆 Certifications

- **CRTO** – Certified Red Team Operator  
- **OSEP** – Offensive Security Experienced Penetration Tester  
- **CRTE** – Certified Red Team Expert  
- **GXPN** – GIAC Exploit Researcher & Advanced Penetration Tester  

---

## 🏗 Lab Setup Recommendation

- Windows Server Domain Controller (AD environment)  
- Windows 10 client machines  
- Kali Linux attacker VM  
- Optional: SIEM for detection testing  
- Virtualization: VMware Workstation / VirtualBox  

---

## ⚠️ Notes

- Red Teaming is **objective-based, stealthy, and persistence-focused**.  
- Focus on understanding **system internals**, not just tools.  
- Always practice in **authorized environments only**.  

---

## 🚀 Bonus YouTube Channels

- John Hammond – https://www.youtube.com/channel/UCVeW9qkBjo3zosnqUbG7CFw  
- LiveOverflow – https://www.youtube.com/c/LiveOverflow  
- IppSec – https://www.youtube.com/c/IppSec  
- The Cyber Mentor – https://www.youtube.com/c/TheCyberMentor  

---

## 🔴 Advanced Red Teaming Roadmap (Visual)

```mermaid
flowchart TD
    A[Foundations] --> B[Exploit Development]
    B --> C[Active Directory Attacks]
    C --> D[Evasion & Malware Dev]
    D --> E[Command & Control (C2)]
    E --> F[Adversary Emulation]
    F --> G[Cloud Red Teaming]
    G --> H[Initial Access & Social Engineering]
    
    %% Foundations Details
    subgraph Foundations [Foundations]
        A1[Networking: TCP/IP, VPN, SMB, LDAP, Kerberos]
        A2[OS Internals: Windows & Linux]
        A3[Programming: C, C++, Python, PowerShell, Bash]
    end
    A --> A1
    A --> A2
    A --> A3

    %% Exploit Development Details
    subgraph ExploitDev [Exploit Development]
        B1[Buffer Overflow, Heap Exploitation]
        B2[ROP Chains, Shellcode]
        B3[Tools: Exploit Education, Pwn College]
    end
    B --> B1
    B --> B2
    B --> B3

    %% Active Directory Details
    subgraph AD [Active Directory Attacks]
        C1[Kerberoasting, AS-REP, DCSync]
        C2[Golden/Silver Ticket, Delegation Abuse]
        C3[Tools: BloodHound, Rubeus, Impacket]
    end
    C --> C1
    C --> C2
    C --> C3

    %% Evasion & Malware
    subgraph Evasion [Evasion & Malware Dev]
        D1[Process Hollowing, AMSI/EDR Bypass]
        D2[C2 Obfuscation]
        D3[Resources: ired.team, Awesome-Red-Team]
    end
    D --> D1
    D --> D2
    D --> D3

    %% Command & Control
    subgraph C2 [Command & Control]
        E1[Beacon customization, Traffic shaping]
        E2[Frameworks: Sliver, Havoc]
    end
    E --> E1
    E --> E2

    %% Adversary Emulation
    subgraph Adversary [Adversary Emulation]
        F1[MITRE ATT&CK mapping]
        F2[Threat Intelligence: Mandiant, CrowdStrike]
    end
    F --> F1
    F --> F2

    %% Cloud
    subgraph Cloud [Cloud Red Teaming]
        G1[AWS IAM & Lambda]
        G2[Azure AD & Conditional Access]
    end
    G --> G1
    G --> G2

    %% Initial Access & Social Engineering
    subgraph Social [Initial Access & Social Engineering]
        H1[Phishing, Macro Payloads]
        H2[Evilginx2, SET]
    end
    H --> H1
    H --> H2
```

---

*This roadmap is designed to guide security professionals from a strong foundational knowledge to advanced Red Teaming and Adversary Emulation skills.*
