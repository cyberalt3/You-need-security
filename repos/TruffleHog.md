# TruffleHog

<p align="center">
  <a href="https://github.com/trufflesecurity/trufflehog">
    <img src="https://img.shields.io/github/stars/trufflesecurity/trufflehog?style=for-the-badge&color=yellow" alt="GitHub Stars">
  </a>
  <a href="https://github.com/trufflesecurity/trufflehog/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/trufflesecurity/trufflehog?style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/trufflesecurity/trufflehog">
    <img src="https://img.shields.io/badge/language-Go-00ADD8?style=for-the-badge" alt="Language">
  </a>
</p>

> ⭐ **29,595 stars** | 🔗 [github.com/trufflesecurity/trufflehog](https://github.com/trufflesecurity/trufflehog)

## What is TruffleHog?

**TruffleHog** is an open-source credential scanner developed by **Truffle Security**. It finds, verifies, and analyzes leaked credentials across your code repositories, file systems, S3 buckets, CI/CD systems, and more. Unlike basic regex scanners, TruffleHog actively **verifies** that discovered credentials are still valid, reducing false positives dramatically.

## What is it for?

TruffleHog is built for **secret detection and credential leak prevention**:

- **Find leaked secrets** — API keys, passwords, tokens, private keys, and other credentials
- **Verify credentials** — Automatically check if discovered secrets are still active and valid
- **Scan Git history** — Deep scan through every commit in a repository's history, not just the current state
- **Monitor CI/CD** — Detect secrets that may have leaked through build logs and pipeline artifacts
- **Protect cloud storage** — Scan S3 buckets and other cloud storage for exposed credentials

## How Does It Work?

1. **Source Configuration** — Point TruffleHog at a Git repo, filesystem, S3 bucket, Docker image, or other source
2. **Deep Scanning** — The tool analyzes all content, including Git history (every commit, branch, and tag)
3. **Pattern Matching** — Over 800 credential detectors identify specific secret types (AWS keys, GitHub tokens, Stripe keys, etc.)
4. **Verification** — Each discovered credential is tested against the respective service API to confirm it's valid
5. **Reporting** — Results show the credential type, where it was found, verification status, and the exact commit/file location

```bash
# Scan a Git repository
trufflehog git https://github.com/target/repo.git

# Scan a local filesystem
trufflehog filesystem /path/to/directory

# Scan an S3 bucket
trufflehog s3 --bucket=my-bucket

# Scan a Docker image
trufflehog docker --image=nginx:latest
```

## Key Features

| Feature | Description |
|---|---|
| ✅ Credential Verification | Actively tests if discovered secrets are still valid |
| 📜 Git History Scanning | Scans every commit, not just the latest state |
| 🔍 800+ Detectors | Specific detectors for AWS, GCP, GitHub, Slack, Stripe, and hundreds more |
| ☁️ Cloud Scanning | Scan S3 buckets, GCS, and other cloud storage |
| 🐳 Docker Scanning | Analyze container images for embedded secrets |
| 🔄 CI/CD Integration | Pre-commit hooks, GitHub Actions, and pipeline integration |

## Use Cases

- **Security Teams** — Audit repositories for leaked credentials before they're exploited
- **DevSecOps** — Add pre-commit hooks to prevent secrets from being committed
- **Incident Response** — Quickly determine the scope of a credential leak
- **Compliance** — Demonstrate that credential scanning is part of your SDLC
- **Platform Teams** — Monitor shared infrastructure for exposed secrets

## Topics

`credentials` `devsecops` `secret` `secret-management` `secrets` `security` `security-tools` `trufflehog` `verification`

---

📦 **License:** AGPL-3.0  
🔗 **Repository:** [https://github.com/trufflesecurity/trufflehog](https://github.com/trufflesecurity/trufflehog)
