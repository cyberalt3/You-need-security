# Codex Security

<p align="center">
  <a href="https://github.com/openai/codex-security">
    <img src="https://img.shields.io/github/stars/openai/codex-security?style=for-the-badge&color=yellow" alt="GitHub Stars">
  </a>
  <a href="https://github.com/openai/codex-security/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/openai/codex-security?style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/openai/codex-security">
    <img src="https://img.shields.io/badge/language-TypeScript-3178C6?style=for-the-badge" alt="Language">
  </a>
</p>

> ⭐ **14,309 stars** | 🔗 [github.com/openai/codex-security](https://github.com/openai/codex-security)

## What is Codex Security?

**Codex Security** is OpenAI's security CLI and TypeScript SDK for finding, validating, and fixing security vulnerabilities. Built by the **OpenAI** team, it provides both a command-line interface and a programmatic SDK for integrating AI-powered security scanning into development workflows.

## What is it for?

Codex Security brings **AI-powered vulnerability scanning** to the command line and SDK:

- **CLI vulnerability scanning** — Scan codebases for security issues directly from the terminal
- **Automated validation** — AI validates findings to reduce false positives
- **Fix generation** — Automatically generates code fixes for detected vulnerabilities
- **SDK integration** — TypeScript SDK for building custom security tooling
- **CI/CD ready** — Designed to run in automated pipelines

## How Does It Work?

1. **Installation** — Install via npm: `npm install @openai/codex-security`
2. **Scanning** — Run the CLI against your codebase or integrate the SDK into your tools
3. **AI Analysis** — Codex models analyze code for security vulnerabilities, understanding context and intent
4. **Validation** — Each finding is validated by the AI to confirm it's a real vulnerability
5. **Fix Generation** — For confirmed vulnerabilities, Codex generates suggested code fixes
6. **Reporting** — Output in multiple formats for integration with existing security workflows

```bash
# Install
npm install -g @openai/codex-security

# Scan a project
codex-security scan .

# Scan and auto-fix
codex-security scan --fix .
```

## Key Features

| Feature | Description |
|---|---|
| 🤖 AI-Powered | Leverages OpenAI's models for intelligent vulnerability detection |
| 🔧 CLI Tool | Full-featured command-line interface for security scanning |
| 📦 TypeScript SDK | Programmatic API for building custom security tools |
| 🛠️ Auto-Fix | Generates code patches for detected vulnerabilities |
| ✅ Validation | AI-driven validation reduces false positives |
| 🔄 CI/CD Ready | Designed for integration into automated pipelines |

## Use Cases

- **Developers** — Scan code for security issues before committing
- **Security Engineers** — Build custom security tools with the TypeScript SDK
- **DevSecOps** — Integrate AI security scanning into CI/CD pipelines
- **Open Source Maintainers** — Automated security review for contributions
- **Enterprise Teams** — Scale security scanning with AI-powered analysis

## Topics

`ai-security` `application-security` `cli` `code-scanning` `codex` `codex-security` `cybersecurity` `devsecops` `openai` `typescript` `vulnerability-scanning`

---

📦 **License:** Apache-2.0  
🔗 **Repository:** [https://github.com/openai/codex-security](https://github.com/openai/codex-security)
