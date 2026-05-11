# 👋 Hi, I'm Abhimanyu Rawat

🔐 **Technical Research & Cyber Security Operations Intern**
🎓 GraySentinel

---

## 🛡️ About Me
Aspiring SOC Analyst with hands-on experience in CVE research,
exploit analysis, IDS rule writing, and Blue Team operations.

---

## 🔬 Security Research

| Project | Description | Tools Used |
|---------|-------------|------------|
| [CVE-2022-30190 Follina](link-to-repo) | Full exploit chain lab: MSDT RCE, Suricata IDS detection | Kali Linux, Suricata, Python |
| [CVE-2026-31431 Copy Fail](https://github.com/u1tr0nex/CVE-2026-31431-CopyFail-Lab) | Linux Kernel LPE via `algif_aead` page-cache overwrite — root escalation confirmed on `6.18.12+kali-amd64` | Kali Linux, Python, auditd |

---

## 🧪 Latest Lab — CVE-2026-31431 "Copy Fail"

> 🔴 **CVSS 7.8 (High)** — Linux Kernel Local Privilege Escalation — Disclosed April 29, 2026

**Kernel tested:** `6.18.12+kali-amd64` &nbsp;|&nbsp; **Lab date:** May 2026

**Key findings:**
- ✅ Confirmed LPE — `uid=1000` escalated to `uid=0` (root) via `/etc/passwd` page-cache overwrite
- ✅ Zero on-disk trace — file-integrity tools (AIDE, Tripwire) report system as clean
- ⚠️ `su kali` failed due to PAM `loginuid` re-validation — `sudo -u root /bin/bash` succeeded
- ✅ Mitigation verified: `install algif_aead /bin/false` in `modprobe.d`
- ✅ Demonstrated `blacklist` directive is insufficient vs `install /bin/false`
- ✅ auditd detection rule captures `algif_aead` MODULE_LOAD as IOC

📂 **[Full Lab Documentation & PoC →](https://github.com/u1tr0nex/CVE-2026-31431-CopyFail-Lab)**

---

## 🧰 Skills

`Suricata IDS` `MITRE ATT&CK` `CVE Research` `Kali Linux`
`Log Analysis` `Network Forensics` `SIEM` `Python`
`Linux Kernel Security` `Privilege Escalation` `Blue Team Operations`

---

## 📫 Connect with Me
[![LinkedIn](https://img.shields.io/badge/LinkedIn-blue?logo=linkedin)](https://www.linkedin.com/in/abhimanyu-rawat-3a4754161/)

---

> ⚠️ All security research is conducted on isolated, researcher-owned systems for **defensive and educational purposes only**.
