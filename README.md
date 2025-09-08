# CyberDrain CIS Baseline repository

This repostiroy has been created by CyberDrain in collaberation with @IntuneAdmin. For more OSS baselines check out Jan's work at https://github.com/IntuneAdmin/IntuneBaselines and wolkenman.nl. 

This repository contains **CIS Benchmark-aligned configuration policies** for **Microsoft Intune (Endpoint Manager)**, focused on securing **Windows 10/11** environments.
All policies are provided in **JSON format** for easy import using CyberDrain's CIPP Platform, or for usage with IntuneManagement.

---

## 📂 Repository Structure

```
CIS Microsoft Intune for Windows/
├── CIS Microsoft Intune for Windows Level 1/
│   ├── CISv4 - WIN - L1 - ASR Block Adobe Reader from creating child processes.json
│   ├── CISv4 - WIN - L1 - ASR Block Office applications from injecting code into other processes.json
│   ├── CISv4 - WIN - L1 - Account Logon Audit Credential Validation.json
│   ├── CISv4 - WIN - L1 - User Account Control Run all administrators in Admin Approval Mode.json
│   └── ... (many more Level 1 baseline policies)
│
└── CIS Microsoft Intune for Windows Level Bitlocker/
    ├── CISv4 - WIN - BL - Require Device Encryption.json
    ├── CISv4 - WIN - BL - Deny write access to removable drives not protected by BitLocker.json
    ├── CISv4 - WIN - BL - Require additional authentication at startup.json
    └── ... (BitLocker encryption & recovery policies)
```


## ⚠️ Notes & Recommendations

* These policies are aligned with **CIS Microsoft Windows 10/11 Benchmark v4.x**.
* Always test policies in a **pilot group** before rolling them out to production.
* Some settings (e.g., BitLocker recovery options, ASR rules) may require hardware/firmware support.
* Adjust configurations if needed for compatibility with your environment.

---

## 📖 References

* [CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks)
* [Microsoft Intune Documentation](https://learn.microsoft.com/mem/intune/)
* [BitLocker Overview](https://learn.microsoft.com/windows/security/information-protection/bitlocker/bitlocker-overview)
