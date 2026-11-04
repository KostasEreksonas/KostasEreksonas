## Hi, I'm Kostas 👋

**Security researcher focused on IoT devices, proprietary network protocols and Android applications.**
I take cheap embedded devices apart at API and network layers, search meticulously for gaps in device security, and build the tooling to prove it.

Mažeikiai/Klaipėda, Lithuania. Open to **penetration testing / security research** roles (on-site, remote or relocation)

---

### Vulnerability research

| Finding | Target | Repo |
|:-------:|:------:|:----:|
| Hardcoded AES-CBC key/salt, all-zero IV, 1-iteration PBKDF2 for local data | Perenio Peifc01 camera's Android app | [perenio_app_analysis](https://github.com/KostasEreksonas/perenio_app_analysis) |
| Hardcoded cloud API access/secret keys, unchanged across app versions 3.7–3.20 | TP-Link Tapo Android app | [Tapo_application_analysis](https://github.com/KostasEreksonas/Tapo_application_analysis) |
| Full black-box assessment: CVE reproduction, obfuscated JS web client, Sofia hash cracker | Besder 6024PB-XMA501 IP camera | [Besder investigation](https://github.com/KostasEreksonas/Besder-6024PB-XMA501-ip-camera-security-investigation) |

### Reproduced vulnerabilities

| CVE ID | Description | Target | Repo |
|:------:|:-----------:|:------:|:----:|
|**CVE-2024-3765**| Authentication bypass vulnerability in DVRIP/Sofia protocol |Xiongmai XM530 based IP camera| [DVRIP hash cracker](https://github.com/KostasEreksonas/DVRIP_hash_cracker) |
| **CVE-2025-65856** | Unauthenticated ONVIF access to device info and live video | Xiongmai XM530 based IP camera | [XM_ONVIF_auth_bypass](https://github.com/KostasEreksonas/XM_ONVIF_auth_bypass) |

### Protocol reverse engineering & tooling

- **[DVRIP protocol analysis](https://github.com/KostasEreksonas/DVRIP_analysis)** — reverse-engineered the DVRIP/Sofia protocol used by budget IP cameras; Lua Wireshark dissector that parses headers and JSON payloads and rebuilds audio/video into a playable file.
- **[Tapo protocol analysis](https://github.com/KostasEreksonas/Tapo_protocol_analysis)** — Lua Wireshark dissector for TP-Link Tapo's proprietary discovery, control, media and keep-alive traffic.
- **[Perenio protocol analysis](https://github.com/KostasEreksonas/perenio_app_analysis)** - RTP/RTSP stream reconstruction in Python (H.264 video, L16 audio) from raw packet captures.

### Research & publications

- [**Implementation-level benchmark of ETSI GS QKD 004 and 014 key-delivery interfaces in NS-3/QKDNetSim**](https://www.sciencedirect.com/science/article/pii/S1573427726000159) — *Optical Switching and Networking* (Elsevier), 2026.
- ML-based network intrusion detection (XGBoost + autoencoders):
    * [EDA on CSE-CIC-IDS2018](https://github.com/KostasEreksonas/NIDS_EDA/blob/main/CSE_CIC_IDS2018/README.md)
    * [Flow analysis web UI](https://github.com/KostasEreksonas/Flow_analysis)
- [Post-quantum cryptography inventorization on Linux systems with Rust](https://github.com/KostasEreksonas/crypto_analysis)

### Toolbox

1. **Reverse engineering & API/network analysis:**:
    * Ghidra · JADX · Frida · Wireshark · Scapy · Nmap · BurpSuite · Mitmproxy
2. **Languages:**:
    * Python · Rust · Lua · JavaScript · Bash
3. **Other:**:
    * Linux (Arch, Gentoo) · Docker · FastAPI · PyTorch / TensorFlow

### Contact information

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kostasereksonas/)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:k.ereksonas@gmail.com)
[![ORCID](https://img.shields.io/badge/ORCID-A6CE39?style=for-the-badge&logo=orcid&logoColor=white)](https://orcid.org/0009-0009-7822-3531)
[![TryHackMe](https://img.shields.io/badge/TryHackMe-212C42?style=for-the-badge&logo=tryhackme&logoColor=white)](https://tryhackme.com/r/p/kostasereksonas9)
[![Medium](https://img.shields.io/badge/Medium-000000?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@kostasereksonas)
