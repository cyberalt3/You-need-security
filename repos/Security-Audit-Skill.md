# Security Audit Skill

<p align="center">
  <a href="https://github.com/cloudflare/security-audit-skill">
    <img src="https://img.shields.io/github/stars/cloudflare/security-audit-skill?style=for-the-badge&color=yellow" alt="GitHub Stars">
  </a>
  <a href="https://github.com/cloudflare/security-audit-skill/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/cloudflare/security-audit-skill?style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/cloudflare/security-audit-skill">
    <img src="https://img.shields.io/badge/language-JavaScript-yellow?style=for-the-badge" alt="Language">
  </a>
</p>

> ⭐ **77,484 stars** | 🔗 [github.com/cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill)

## What is Security Audit Skill?

**Security Audit Skill** is a coding-agent skill developed by **Cloudflare** that enables multi-phase security audits with independently verified, machine-readable findings. It is designed to be integrated into AI coding agents (like Claude Code, Codex, Cursor, etc.) to give them the ability to perform thorough security audits of codebases.

## What is it for?

This skill transforms any compatible AI coding agent into a **security auditor**. It provides a structured methodology for:

- **Multi-phase security auditing** of source code repositories
- **Independently verifiable findings** — each vulnerability is validated, not just flagged
- **Machine-readable output** — findings are structured for downstream automation
- **Comprehensive coverage** — examines code for injection flaws, authentication issues, authorization bypasses, data exposure, and more

## How Does It Work?

1. **Skill Installation** — The skill is added to a compatible AI coding agent (e.g., as a Claude Code skill or Codex plugin)
2. **Phase 1: Reconnaissance** — The agent maps the codebase architecture, identifying security-relevant components (auth, input handling, data storage, API endpoints)
3. **Phase 2: Deep Analysis** — Each identified component is analyzed for known vulnerability patterns (OWASP Top 10, CWEs, etc.)
4. **Phase 3: Verification** — Findings are independently verified — the agent cross-checks each finding to reduce false positives
5. **Phase 4: Reporting** — A structured, machine-readable report is generated with severity ratings, affected code locations, and remediation guidance

## Key Features

| Feature | Description |
|---|---|
| 🔍 Multi-Phase Audit | Systematic reconnaissance → analysis → verification → reporting pipeline |
| ✅ Independent Verification | Each finding is cross-validated to minimize false positives |
| 📋 Machine-Readable Output | Structured findings ready for ticketing systems and dashboards |
| 🔌 Agent-Native Design | Built to plug into AI coding agents, not standalone CLI |
| ☁️ Cloudflare-Backed | Developed by Cloudflare's security team with production-grade rigor |

## Use Cases

- **Security Teams** — Augment manual code reviews with automated AI-powered auditing
- **Developer Teams** — Run security audits as part of the code review process
- **Compliance** — Generate evidence of security reviews for audits and certifications
- **Open Source Maintainers** — Quickly assess the security posture of contributions

## Topics

`security-audit` `coding-agent` `cloudflare` `vulnerability-detection` `code-review`

---

📦 **License:** MIT  
🔗 **Repository:** [https://github.com/cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill)
