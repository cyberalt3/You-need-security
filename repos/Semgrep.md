# Semgrep

<p align="center">
  <a href="https://github.com/semgrep/semgrep">
    <img src="https://img.shields.io/github/stars/semgrep/semgrep?style=for-the-badge&color=yellow" alt="GitHub Stars">
  </a>
  <a href="https://github.com/semgrep/semgrep/blob/develop/LICENSE">
    <img src="https://img.shields.io/github/license/semgrep/semgrep?style=for-the-badge" alt="License">
  </a>
  <a href="https://github.com/semgrep/semgrep">
    <img src="https://img.shields.io/badge/language-C-A8B9CC?style=for-the-badge" alt="Language">
  </a>
</p>

> ⭐ **17,909 stars** | 🔗 [github.com/semgrep/semgrep](https://github.com/semgrep/semgrep)

## What is Semgrep?

**Semgrep** is a lightweight, fast static analysis tool that supports many programming languages. It allows you to find bug variants and security vulnerabilities using patterns that look like source code — no complex query languages needed. Created by **Semgrep, Inc.** (formerly r2c), it's used by thousands of organizations for SAST (Static Application Security Testing).

## What is it for?

Semgrep is a **developer-friendly static analysis engine** for:

- **Security vulnerability detection** — Find SQL injection, XSS, command injection, and other OWASP Top 10 issues
- **Bug finding** — Detect logic errors, anti-patterns, and coding mistakes
- **Code standards enforcement** — Ensure consistent coding patterns across teams
- **Custom rule creation** — Write rules that look like the code you're searching for
- **Multi-language support** — Python, JavaScript, TypeScript, Java, Go, C, Ruby, and 20+ more languages

## How Does It Work?

1. **Rule Definition** — Write rules using Semgrep's pattern syntax (looks like source code with metavariables like `$VAR`)
2. **Scanning** — Run Semgrep against your codebase, CI/CD pipeline, or IDE
3. **AST Matching** — Unlike regex-based tools, Semgrep parses code into an AST and matches patterns structurally
4. **Results** — Findings include the matched code, rule description, severity, and fix suggestions
5. **Integration** — Output in SARIF, JSON, or text; integrates with GitHub, GitLab, and other platforms

```bash
# Run with default security rules
semgrep --config auto .

# Run with specific rules
semgrep --config p/owasp-top-ten .

# Run a custom rule
semgrep --config my-rules/ .
```

## Key Features

| Feature | Description |
|---|---|
| 📝 Code-Like Rules | Write rules that look like the code you're matching — intuitive and fast |
| 🌐 20+ Languages | Python, JS/TS, Java, Go, C, C#, Ruby, PHP, Kotlin, Rust, and more |
| 🌳 AST-Based | Structural matching, not regex — fewer false positives |
| ⚡ Fast | Scans large codebases in seconds |
| 🔄 CI/CD Native | First-class support for GitHub Actions, GitLab CI, and more |
| 📚 Community Rules | Thousands of community-maintained rules for security and best practices |

## Use Cases

- **Application Security** — Automate SAST in CI/CD pipelines for every pull request
- **Developer Teams** — Enforce coding standards and catch bugs early
- **Security Researchers** — Write custom rules to find novel vulnerability patterns
- **Code Review** — Augment manual code reviews with automated checks
- **Compliance** — Enforce regulatory requirements through automated code scanning

## Topics

`sast` `static-analysis` `static-code-analysis` `semgrep` `python` `javascript` `java` `go` `ruby` `typescript`

---

📦 **License:** LGPL-2.1  
🔗 **Repository:** [https://github.com/semgrep/semgrep](https://github.com/semgrep/semgrep)
