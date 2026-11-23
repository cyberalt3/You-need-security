# Trivy

<p align="center">
  <a href="https://github.com/aquasecurity/trivy">
    <img src="https://img.shields.io/github/stars/aquasecurity/trivy?style=for-the-badge&color=yellow" alt="GitHub Stars">
  </a>
  <a href="https://github.com/aquasecurity/trivy/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/aquasecurity/trivy?style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/aquasecurity/trivy">
    <img src="https://img.shields.io/badge/language-Go-00ADD8?style=for-the-badge" alt="Language">
  </a>
</p>

> ⭐ **39,656 stars** | 🔗 [github.com/aquasecurity/trivy](https://github.com/aquasecurity/trivy)

## What is Trivy?

**Trivy** is a comprehensive, fast, and easy-to-use security scanner developed by **Aqua Security**. It is the most popular open-source vulnerability scanner for containers, Kubernetes, code repositories, cloud environments, and infrastructure-as-code (IaC). Trivy detects vulnerabilities, misconfigurations, secrets, and generates Software Bill of Materials (SBOM).

## What is it for?

Trivy is an **all-in-one security scanner** that covers the entire software supply chain:

- **Container Image Scanning** — Find known CVEs in OS packages and application dependencies
- **Filesystem & Repository Scanning** — Scan local projects or Git repos for vulnerabilities
- **IaC Scanning** — Detect misconfigurations in Terraform, CloudFormation, Dockerfiles, Kubernetes manifests, and more
- **Kubernetes Scanning** — Audit running clusters for security issues
- **Secret Detection** — Find hardcoded passwords, API keys, and tokens
- **SBOM Generation** — Generate Software Bill of Materials in SPDX and CycloneDX formats

## How Does It Work?

1. **Installation** — Available as a standalone binary, Docker image, or integrated into CI/CD (GitHub Actions, GitLab CI, Jenkins, etc.)
2. **Target Selection** — Specify what to scan: a container image, filesystem path, Git repository, Kubernetes cluster, or cloud account
3. **Scanning** — Trivy analyzes the target against its vulnerability database (updated from NVD, vendor advisories, and other sources)
4. **Detection** — Vulnerabilities are matched by package name and version; misconfigurations are checked against security best practices (CIS Benchmarks, etc.)
5. **Reporting** — Results are output in multiple formats: table, JSON, SARIF, CycloneDX, SPDX, and more

```bash
# Scan a container image
trivy image nginx:latest

# Scan a local project
trivy fs /path/to/project

# Scan IaC files
trivy config /path/to/terraform

# Scan a Kubernetes cluster
trivy k8s --report summary
```

## Key Features

| Feature | Description |
|---|---|
| 📦 Container Scanning | Scan Docker/OCI images for OS and application vulnerabilities |
| 🔧 IaC Scanning | Detect misconfigurations in Terraform, Dockerfile, K8s manifests, etc. |
| 🔑 Secret Detection | Find hardcoded credentials, API keys, tokens |
| ☸️ Kubernetes | Audit running clusters for security posture |
| 📄 SBOM | Generate SPDX and CycloneDX Software Bill of Materials |
| ⚡ Fast & Easy | Single binary, zero configuration needed, offline-capable |
| 🔄 CI/CD Ready | First-class GitHub Actions, GitLab CI, and Jenkins integrations |

## Use Cases

- **DevSecOps Teams** — Shift-left security by scanning in CI/CD pipelines
- **Platform Engineers** — Enforce image security policies in container registries
- **Compliance Teams** — Generate SBOMs and vulnerability reports for audits
- **Cloud Security** — Scan cloud infrastructure and IaC for misconfigurations
- **Kubernetes Administrators** — Continuously monitor cluster security posture

## Topics

`containers` `devsecops` `docker` `kubernetes` `vulnerability` `vulnerability-scanners` `infrastructure-as-code` `security-tools` `sbom`

---

📦 **License:** Apache-2.0  
🔗 **Repository:** [https://github.com/aquasecurity/trivy](https://github.com/aquasecurity/trivy)
