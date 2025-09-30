# 🛡️ Security Policy for AnimeStream

Thank you for helping keep **AnimeStream** secure. Your efforts to responsibly disclose potential security issues are greatly appreciated by the project maintainers and the wider community.

This document outlines the **security policy** for the open-source project [**AnimeStream**](https://github.com/frostnova721/animestream), a Flutter-based application for streaming and downloading anime content.

---

## 🔍 Scope of This Policy

This policy applies **only** to the following components:

- The **source code** in the `frostnova721/animestream` GitHub repository (including all branches and tags).
- The **compiled mobile application** distributed via official channels (e.g., GitHub Releases).
- Any **local data handling**, such as:
  - Storage of user preferences (e.g., via `shared_preferences`)
  - Caching of metadata or images
  - Network requests made by the app (e.g., to third-party anime APIs or scrapers)

### ❌ Out of Scope
The following are **not covered** by this policy and should **not** be reported as security vulnerabilities:
- Content legality, copyright, or DMCA-related concerns.
- Security or reliability of **external websites, APIs, or streaming sources** that the app may access (e.g., third-party anime hosts). These are outside the project’s control.
- General feature requests, performance issues, or non-security-related bugs (please use [GitHub Issues](https://github.com/frostnova721/animestream/issues) for those).
- Issues in forked or modified versions of the app not maintained by the original author.

---

## 📬 How to Report a Security Vulnerability

If you believe you’ve discovered a **security vulnerability** in AnimeStream, **do not** create a public GitHub issue, pull request, or discussion post. Public disclosure could put users at risk.

Instead, please follow the **responsible disclosure process** below.

### ✅ Authorized Contact Methods

You may report vulnerabilities **only** through  these following **verified channels**:

> 🔐 **Encryption strongly recommended**:  
> If you have PGP/GPG, please encrypt your message using the maintainer’s public key (available upon request).  
> At minimum, **avoid sending sensitive exploit code or credentials in plain text**.

#### 1. **Discord (Direct Message Only) (⚠️PREFERDE!!!)**
Contact the main developer directly on Discord:  
👤 **`frostnova721`** (User ID: `721684932370432041`)
Always be respectful !

> ⚠️ **Important**:  
> - Only message the **exact username** above.  
> - Do **not** post in public servers, channels, or mention the vulnerability in group chats.  
> - Verify the user’s identity by confirming their GitHub profile link or asking for a signed message.

> ❗ **Do not contact any other accounts** claiming to represent the project—only the verified maintainer listed above is authorized to receive vulnerability reports.

---

## 📝 What to Include in Your Report

To help us assess and resolve the issue quickly, please provide as much of the following as possible:

- **Summary**: A clear, concise description of the vulnerability.
- **Impact**: What could an attacker do? (e.g., access local files, leak user data, execute arbitrary code, etc.)
- **Affected Version(s)**: Which release or Git commit is vulnerable? (e.g., `v1.2.0`, `main@abc123d`)
- **Steps to Reproduce**: Detailed instructions or a proof-of-concept (PoC) script.
- **Environment**: OS (Android/iOS), device type, Flutter version (if relevant).
- **Proposed Fix** (optional): Suggestions for mitigation or patching.
- **Your Contact Info**: So we can follow up (email or Discord username).

---

## ⏳ Our Commitment to You

Upon receiving your report, we will:

1. **Acknowledge** your submission within **5 business days**.
2. **Investigate** the issue and determine its validity and severity.
3. **Keep you informed** of our progress, including timelines for a fix.
4. **Coordinate disclosure** with you before making any public announcement.
5. **Credit you** in the release notes or security advisory (unless you request anonymity).

We ask for a **reasonable disclosure window** (typically **30–60 days**) to develop, test, and deploy a fix before any public disclosure.

---

## 🤝 Responsible Disclosure Expectations

By reporting a vulnerability under this policy, you agree to:

- **Not exploit** the vulnerability beyond what is necessary for verification.
- **Not share, publish, or distribute** any details of the vulnerability until a fix is released and coordinated with the maintainer.
- **Not use automated scanners or aggressive testing** that could disrupt service or user data.
- **Act in good faith** to protect the project and its users.

Violations of these expectations may result in the report being deprioritized or ignored.

---

## 🚀 Patching & Disclosure

Once a vulnerability is confirmed:
- A patch will be developed and tested.
- A new version of the app will be released on [GitHub Releases](https://github.com/frostnova721/animestream/releases).
- A **security advisory** may be published via [GitHub Security Advisories](https://github.com/frostnova721/animestream/security/advisories) (if applicable).
- High-severity issues may be assigned a **CVE ID** upon request or through GitHub’s integration.

---

## 📜 License & Disclaimer

AnimeStream is provided **"as is"**, without warranty of any kind. The project **does not host or distribute copyrighted content**—it acts as a client to publicly available third-party sources. Users are solely responsible for compliance with local laws.

The maintainer(s) are **not liable** for any damages arising from the use or misuse of this software.

---

> ❤️ Thank you for helping make AnimeStream safer for everyone.

*Last updated: April 2025*  
*Maintained by: frostnova721*

---

### How to Add This to Your Repository

1. In your local clone of the repo, create a new file:  
   ```bash
   touch SECURITY.md
   ```
2. Paste the content above into `SECURITY.md`.
3. Commit and push:
   ```bash
   git add SECURITY.md
   git commit -m "Add security policy"
   git push origin main
   ```

GitHub will automatically recognize this file and display a **Security tab** on your repository homepage, improving trust and transparency.

Let me know if you'd like a shorter version or one formatted for GitHub Pages!
