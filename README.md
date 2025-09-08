# CyberDrain CIS Baseline Repository

This repository has been created by **CyberDrain** in collaboration with [@IntuneAdmin](https://github.com/IntuneAdmin).
For additional OSS baselines, check out Jan’s work at [Intune Baselines](https://github.com/IntuneAdmin/IntuneBaselines) and [wolkenman.nl](https://wolkenman.nl).

This repository provides **CIS Benchmark–aligned configuration policies** for **Microsoft Intune (Endpoint Manager)**, focusing on securing **Windows 10/11** environments.

All policies are supplied in **JSON format**, making them ready for direct import into the **CyberDrain CIPP Platform** or for usage with **Intune Management**.

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
└── CIS Microsoft Intune for Windows Level BitLocker/
    ├── CISv4 - WIN - BL - Require Device Encryption.json
    ├── CISv4 - WIN - BL - Deny write access to removable drives not protected by BitLocker.json
    ├── CISv4 - WIN - BL - Require additional authentication at startup.json
    └── ... (BitLocker encryption & recovery policies)
```

---

## ⚠️ Notes & Recommendations

* These policies are aligned with **CIS Microsoft Windows 10/11 Benchmark v4.x**.
* Always test policies in a **pilot group** before production rollout.
* Some settings (e.g., **BitLocker recovery options, ASR rules**) may depend on hardware/firmware compatibility.
* Adjust policies where needed to match your specific organizational environment.

---

## 📖 References

* [CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks)
* [Microsoft Intune Documentation](https://learn.microsoft.com/mem/intune/)
* [BitLocker Overview](https://learn.microsoft.com/windows/security/information-protection/bitlocker/bitlocker-overview)

---

## 💡 Reasoning & Contribution

This repository is an **open-source library** created for use by everyone.
It was built in collaboration with an expert in **CIS Intune templates** and will be continuously maintained by CyberDrain to stay up to date with CIS Benchmark changes.

* Completely **open source (MIT license)**.
* Community contributions are welcome — we accept **pull requests**.
* Designed to help MSPs and sysadmins deploy **hardened, standardized baselines** quickly and reliably.

