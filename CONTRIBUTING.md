<div align="center">
```
╔══════════════════════════════════════════════════════════════════════════════════╗
║ 01101000 01100001 01100011 01101011 01100101 01110010 01110011 01101000 01101001 ║
║ 10110100 11001010 00110110 10010011 11010110 00110101 01001011 10101100 11100101 ║
║                                                                                  ║
║          🔐  ·  S C E P - A I  ·  P A S S W O R D  E N T R O P Y  ·  🔐          ║
║                  ─────────────────────────────────────────────                   ║
║                         P  O  W  E  R  E  D     B  Y     A  I                    ║
║                                                                                  ║
║ 01110000 01100001 01110011 01110011 01110111 01101111 01110010 01100100 01110011 ║
║ 11001010 00110110 10110001 01101110 10010011 11010110 00110101 10110100 01001011 ║
╚══════════════════════════════════════════════════════════════════════════════════╝
```

<br>

[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-00ff88.svg?style=for-the-badge&logo=github)](../../pulls)
[![Contributors](https://img.shields.io/github/contributors/jakyunknown/SCEP-AI?style=for-the-badge&color=ff6b6b&logo=github)](../../graphs/contributors)
[![Issues](https://img.shields.io/github/issues/jakyunknown/SCEP-AI?style=for-the-badge&color=ffd93d)](../../issues)
[![License](https://img.shields.io/github/license/jakyunkown/SCEP-AI?style=for-the-badge&color=6bcbff)](./LICENSE)



> *"Weak passwords are the #1 attack vector. Let's fix that — together."*

</div>

<br>

---

<br>

## 👾 Hey, you found the contributing guide!

Pull up a chair. **SCEP-AI** uses AI to analyze password entropy and tell you — with brutal honesty — how crackable your password is. It's a security tool, which means the code needs to be rock solid. That's where you come in.

This doc covers everything you need to go from zero → merged PR. Don't skip it. It's short, we promise.

<br>

---

<br>

## 🗺️ Navigation

<div align="center">

| 🔴 | 🟡 | 🟢 |
|:---:|:---:|:---:|
| [Code of Conduct](#-code-of-conduct) | [Dev Setup](#-development-setup) | [Submit a PR](#-submitting-a-pull-request) |
| [Report a Bug](#-reporting-bugs) | [Branch Names](#-branch-naming) | [Commit Style](#-commit-messages) |
| [Request a Feature](#-feature-requests) | [Code Style](#-code-style) | [Testing](#-testing) |
| [Security Policy](#-security) | [Questions](#-questions) | [Thank You](#-thank-you) |

</div>

<br>

---

<br>

## 🤝 Code of Conduct

```
┌─ RULE #1 ──────────────────────────────────────────────────────┐
│  Don't be a jerk. Seriously. That's it.                        │
└────────────────────────────────────────────────────────────────┘
```

We're building a security tool used by real people. We take the project seriously, and we take our community seriously. Be inclusive, be kind, give feedback that helps people grow. Abusive behavior = immediate ban.

<br>

---

<br>

## 🚀 Getting Started

```bash
#  ╔══════════════════════════════════════╗
#  ║   STEP 1 — Fork it on GitHub         ║
#  ╚══════════════════════════════════════╝

#  ╔══════════════════════════════════════╗
#  ║   STEP 2 — Clone your fork           ║
#  ╚══════════════════════════════════════╝
git clone https://github.com/YOUR_USERNAME/SCEP-AI.git
cd SCEP-AI

#  ╔══════════════════════════════════════╗
#  ║   STEP 3 — Hook up upstream          ║
#  ╚══════════════════════════════════════╝
git remote add upstream https://github.com/ORIGINAL_OWNER/SCEP-AI.git
git remote -v  # verify it looks right

#  ╔══════════════════════════════════════╗
#  ║   STEP 4 — Stay in sync (always!)    ║
#  ╚══════════════════════════════════════╝
git fetch upstream && git merge upstream/main
```

<br>

---

<br>

## 🐛 Reporting Bugs

First — check [existing issues](../../issues). Duplicate reports slow everyone down.

If it's new, open an issue and fill this out:

```
╔══════════════════════════════════════════════════════════╗
║  BUG REPORT                                              ║
╠══════════════════════════════════════════════════════════╣
║  Title        │ [Short, specific description]            ║
║  Version      │ [e.g., v1.2.0 or commit abc1234]         ║
╠══════════════════════════════════════════════════════════╣
║  STEPS TO REPRODUCE                                      ║
║  1.                                                      ║
║  2.                                                      ║
║  3.                                                      ║
╠══════════════════════════════════════════════════════════╣
║  Expected  ✅ │                                          ║
║  Actual    ❌ │                                          ║
╠══════════════════════════════════════════════════════════╣
║  OS           │ [macOS / Ubuntu / Windows]               ║
║  Python/Node  │ [version]                                ║
║  Logs         │ [paste relevant output here]             ║
╚══════════════════════════════════════════════════════════╝
```

[→ File a Bug Report](../../issues/new?template=bug_report.md)

<br>

---

<br>

## 💡 Feature Requests

Got a vision for SCEP-AI? We want to hear it.

The best feature requests answer three questions:

```
  WHAT   →  What do you want SCEP-AI to do that it can't today?
  WHY    →  What problem does this solve for users?
  HOW    →  Any ideas on implementation? (optional but appreciated)
```

[→ Open a Feature Request](../../issues/new?template=feature_request.md)

<br>

---

<br>

## 🔧 Development Setup

<details>
<summary>🐍 &nbsp;<b>Python</b></summary>
<br>

```bash
python -m venv .venv
source .venv/bin/activate        # macOS / Linux
# .venv\Scripts\activate         # Windows

pip install -r requirements.txt
pip install -r requirements-dev.txt

python main.py
```

</details>

<details>
<summary>🟨 &nbsp;<b>Node.js</b></summary>
<br>

```bash
npm install
npm run dev       # development
npm run build     # production
```

</details>

<details>
<summary>🐳 &nbsp;<b>Docker</b></summary>
<br>

```bash
docker build -t scep-ai .
docker run -p 8080:8080 scep-ai
```

</details>

<br>

---

<br>

## 📬 Submitting a Pull Request

```
  ┌───┐     ┌───┐     ┌───┐     ┌───┐     ┌───┐     ┌───┐     ┌─────┐
  │ 🌿│────▶│ 🔨│────▶│ ✅│────▶│ 🧹│────▶│ 📝│────▶│ 📤│────▶│ 🎉  │
  └───┘     └───┘     └───┘     └───┘     └───┘     └───┘     └─────┘
  Branch    Code      Test      Lint     Commit     Push      Merged!
```

```bash
git checkout -b feat/your-feature-name   # branch
# ... make your changes ...
pytest && flake8 .                       # test + lint
git commit -m "feat: your message here" # commit
git push origin feat/your-feature-name  # push
# open PR on GitHub → target: main
```

Your PR description should cover:
- **What** changed and **why**
- How it was tested
- `Closes #ISSUE_NUMBER` if applicable

<br>

---

<br>

## 🌿 Branch Naming

| Prefix | When to use | Example |
|--------|-------------|---------|
| `feat/` | New feature or enhancement | `feat/ml-scoring-model` |
| `fix/` | Bug fix | `fix/entropy-negative-value` |
| `docs/` | Documentation only | `docs/add-api-reference` |
| `refactor/` | Code cleanup, no behavior change | `refactor/simplify-tokenizer` |
| `test/` | Adding or fixing tests | `test/unicode-edge-cases` |
| `chore/` | Deps, CI, tooling | `chore/upgrade-torch` |

<br>

---

<br>

## ✍️ Commit Messages

We follow **[Conventional Commits](https://www.conventionalcommits.org/)**.

```
<type>(<scope>): <what you did, present tense>
                  └── not "fixed", not "fixing" — "fix"

[body: explain WHY, not WHAT — the diff shows what]

[footer: BREAKING CHANGE: ... or Closes #123]
```

**Good:**
```bash
feat(entropy): support kanji and emoji character sets
fix(cli): prevent crash on empty stdin input
test(model): cover single-char and max-length edge cases
```

**Bad:**
```bash
stuff
fix bug
FINAL FINAL v2
```

<br>

---

<br>

## 🎨 Code Style

```
  ┌──────────────────────────────────────────────────────────┐
  │  SCEP-AI Core Principle:  Security code must be READ-    │
  │  ABLE. Cleverness is a liability. Clarity is a feature.  │
  └──────────────────────────────────────────────────────────┘
```

- Name things well: `calculate_shannon_entropy()` not `cse()`
- One function = one job
- Comment **why**, not **what** — the code says what, comments explain intent
- Run linting before every commit:

```bash
# Python
black . && flake8 . --max-line-length=100

# JavaScript
npm run lint && npm run format
```

> 💡 Set up a pre-commit hook once and never think about it again.

<br>

---

<br>

## 🧪 Testing

**No tests = no merge.** We're serious. This is a security tool.

```
  Priority matrix for SCEP-AI tests:

  ┌─────────────────────────────┬──────────────────────────────┐
  │  🔴 CRITICAL                │  🟡 IMPORTANT                │
  │  ─────────────────────────  │  ──────────────────────────  │
  │  Entropy math accuracy      │  API input validation        │
  │  Empty / null passwords     │  AI model output bounds      │
  │  Unicode & special chars    │  CLI argument handling       │
  ├─────────────────────────────┼──────────────────────────────┤
  │  🟢 GOOD TO HAVE            │  🔵 BONUS                    │
  │  ─────────────────────────  │  ──────────────────────────  │
  │  Performance benchmarks     │  Visual output formatting    │
  │  Very long passwords        │  i18n / locale handling      │
  └─────────────────────────────┴──────────────────────────────┘
```

```bash
# Python
pytest --cov=scep_ai --cov-report=term-missing

# JavaScript
npm test -- --coverage
```

<br>

---

<br>

## 🔐 Security

```
  ⚠️  DO NOT open a public GitHub issue for vulnerabilities.
```

SCEP-AI processes passwords. A vulnerability here isn't just a bug — it's a risk to real users. Please disclose responsibly:

1. Email maintainers privately (see README for contact info)
2. Or use [GitHub private vulnerability reporting](../../security/advisories/new)
3. Allow **72 hours** for us to respond before any public disclosure

We take every report seriously. Thank you for being responsible.

<br>

---

<br>

## 💬 Questions

```
  Lost?  →  Open a Discussion  →  ../../discussions
  Bug?   →  File an Issue      →  ../../issues
  Docs?  →  Start in README    →  ./README.md
```

No question is too small. We were all beginners once.

<br>

---

<br>

<div align="center">

```
  ╔═══════════════════════════════════════════════════════╗
  ║                                                       ║
  ║   You're not just writing code.                       ║
  ║   You're making passwords stronger for everyone.      ║
  ║                                                       ║
  ║              Thank you for contributing.  🔐          ║
  ║                                                       ║
  ╚═══════════════════════════════════════════════════════╝
```

*Made with ❤️ by the SCEP-AI community*

</div>
