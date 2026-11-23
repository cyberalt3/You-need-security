# ClamAV

<p align="center">
  <a href="https://github.com/Cisco-Talos/clamav">
    <img src="https://img.shields.io/github/stars/Cisco-Talos/clamav?style=for-the-badge&color=yellow" alt="GitHub Stars">
  </a>
  <a href="https://github.com/Cisco-Talos/clamav/blob/main/COPYING">
    <img src="https://img.shields.io/github/license/Cisco-Talos/clamav?style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/Cisco-Talos/clamav">
    <img src="https://img.shields.io/badge/language-C-A8B9CC?style=for-the-badge" alt="Language">
  </a>
</p>

> ⭐ **7,711 stars** | 🔗 [github.com/Cisco-Talos/clamav](https://github.com/Cisco-Talos/clamav)

## What is ClamAV?

**ClamAV** is an open-source antivirus engine maintained by **Cisco Talos**. It is one of the most widely deployed open-source antivirus solutions in the world, used primarily for email gateway scanning, file server protection, and web scanning. ClamAV has been protecting systems for over two decades.

## What is it for?

ClamAV provides **open-source malware detection and antivirus protection**:

- **Email gateway scanning** — Scan email attachments for malware at the mail server level
- **File server protection** — Detect malicious files on shared storage and servers
- **Web scanning** — Inspect files downloaded from the web for threats
- **On-access scanning** — Real-time file scanning as files are accessed
- **Custom signatures** — Create your own malware signatures for targeted detection
- **Multi-format support** — Scans archives (ZIP, RAR, 7z, etc.), documents (PDF, Office), executables, and more

## How Does It Work?

1. **Signature Database** — ClamAV downloads and maintains a database of malware signatures from Cisco Talos
2. **Scanning Engine** — Files are scanned against the signature database using multiple detection techniques
3. **Archive Unpacking** — Compressed files and archives are automatically extracted and scanned recursively
4. **Heuristic Analysis** — Beyond signatures, ClamAV uses heuristics to detect unknown malware variants
5. **Results** — Detected threats are reported with the malware name and signature match

```bash
# Update signature database
freshclam

# Scan a file
clamscan /path/to/file

# Scan a directory recursively
clamscan -r /path/to/directory

# Run as a daemon for real-time scanning
clamd
```

## Key Features

| Feature | Description |
|---|---|
| 🦠 Malware Detection | Detects viruses, trojans, malware, and other threats |
| 📧 Email Scanning | Built for email gateway integration (Postfix, Sendmail, etc.) |
| 📦 Archive Support | Scans inside ZIP, RAR, 7z, TAR, and many archive formats |
| 📄 Document Scanning | Analyzes PDFs, Office documents, and HTML for malicious content |
| 🔄 Auto Updates | `freshclam` daemon keeps signatures up to date automatically |
| 🏭 Production Grade | Deployed by thousands of organizations worldwide for 20+ years |

## Use Cases

- **Mail Servers** — Scan incoming/outgoing email for malware at the gateway
- **File Servers** — Protect shared storage from malicious file uploads
- **Web Applications** — Scan user-uploaded files before accepting them
- **CI/CD Pipelines** — Scan build artifacts for malware before deployment
- **Linux Servers** — Lightweight antivirus protection for server environments

## Topics

`antivirus` `clamav` `malware-detection` `email-security` `file-scanning` `open-source`

---

📦 **License:** GPL-2.0  
🔗 **Repository:** [https://github.com/Cisco-Talos/clamav](https://github.com/Cisco-Talos/clamav)
