# Companion repository — security & release-readiness review

**Repo:** `codethor0/prompting-as-a-programming-language-companion`  
**Review UTC:** **2026-05-03**  
**Reviewer:** automated tooling + manual checklist *(no manuscript changes)*  

---

## 1. Executive summary

Repository visibility remains **PRIVATE**. **`gitleaks`** and **`trufflehog`** were **not installed** on this workstation (**`SECRET_SCAN_TOOL_MISSING`**); install one before widening access or flipping visibility. Heuristic **`grep`** surfaced **two benign hits** (instructional wording + **`.gitignore`** ignore path)—no actionable leaks identified in tracked workbook Markdown.

No forbidden binaries (**.epub**, **.docx**, **.pdf**, **.env**, logs, DB files, **`secrets/`** folders as content) were present in the working tree. Required workbook directories and safety framing in **`README.md`** are present.

**Recommended posture:** **`KEEP_PRIVATE`** until dedicated leak scanners pass **clean**, license posture is chosen, and author explicitly approves any broader sharing.

---

## 2. Repo privacy status *(CLI)*

| Field | Value |
|-------|--------|
| **URL** | https://github.com/codethor0/prompting-as-a-programming-language-companion |
| **`nameWithOwner`** | `codethor0/prompting-as-a-programming-language-companion` |
| **`isPrivate`** | **`true`** |
| **Default branch** | **`main`** |

*(Source: `gh repo view … --json isPrivate,nameWithOwner,url,defaultBranchRef`.)*

---

## 3. Files inspected

- Full tracked tree under `/Users/thor/Projects/prompting-as-a-programming-language-companion` *(excluding **`.git`** from scans)*  
- **`README.md`**, **`PRIVATE-UNTIL-APPROVED.md`**, **`docs/`**, **`workflows/`** for tone alignment  

---

## 4. Secret scan tools used

| Tool | Status |
|------|--------|
| **`gitleaks`** | **Not installed** (`which gitleaks` → empty) |
| **`trufflehog`** | **Not installed** (`which trufflehog` → empty) |

**Recorded:** **`SECRET_SCAN_TOOL_MISSING`** — **no** `gitleaks-report.json` / `trufflehog-report.json` produced.

---

## 5. Secret scan result

**Not executed** — prerequisite tooling absent. **Do not** infer cleanliness from absence of scans.

---

## 6. Basic grep result

Command *(abbreviated)*:

```bash
grep -RInE 'api[_-]?key|password|secret|token|credential|private key|BEGIN RSA|BEGIN OPENSSH|AWS_ACCESS_KEY|GITHUB_TOKEN|customer data|client data|real customer|real client|SOURCE NEEDED|TODO AUTHOR|Before upload|Chapter 99' . --exclude-dir=.git
```

**Hits:**

| Path | Note |
|------|------|
| `workflows/cybersecurity-log-analysis-workflow.md:33` | Instructional phrase **“credential-like strings”** — prompts halt if paste resembles credentials; **not** embedded secrets. |
| `.gitignore:15` | Ignore rule **`secrets/`** — prevents accidental commit of a conventionally named folder; **not** repository content. |

**Assessment:** **No secrets or staging placeholders detected** in workbook prose beyond expected hygiene language.

---

## 7. Forbidden file type check

| Category | Result |
|----------|--------|
| **`*.epub`**, **`*.docx`**, **`*.pdf`** | **None found** *(also blocked via **`.gitignore`**)* |
| **`.env`** | **None found** |
| **`*.log`**, **`*.sqlite`**, **`*.db`** | **None found** |
| **`secrets/`**, **`private/`**, **`exports/`**, **`kdp/`**, **`manuscript/`** as committed dirs | **Do not exist** in tree *(exit **non-zero** from `ls` — expected)* |

---

## 8. Workbook structure check

| Path | Present |
|------|---------|
| `README.md` | **YES** |
| `PRIVATE-UNTIL-APPROVED.md` | **YES** |
| `BOOK-COMPANION-NOTES.md` | **YES** |
| `RELEASE-CHECKLIST.md` | **YES** |
| `templates/` | **YES** |
| `workflows/` | **YES** |
| `examples/` | **YES** |
| `checklists/` | **YES** |
| `fixtures/` | **YES** |
| `docs/` | **YES** |

---

## 9. Safety-language check *(README + companion norms)*

| Expectation | Evidence |
|-------------|----------|
| Private **draft** posture | **`README`** header “Private draft — **NOT PUBLIC / NOT FINAL**” |
| **Fictional/sanitized** examples | **`README`** § included / excluded |
| **No real identifiable records** | **`README`** exclusions list |
| **Practice aid, not source of truth** | **`README`** safety rule **#1** (“practice aids”) |
| **Not professional advice** | **`README`** disclaimer paragraph |
| **Human review** implied | Safety rule **#4**, templates/workflows carry **`DRAFT — HUMAN_REVIEW_REQUIRED`** |
| **Validation** | **`README`** mentions validation / tool output as artefact |
| **STOP_CONDITIONS** preserved | **`README`** § included bullet + workflow/template norms |

---

## 10. Remaining blockers before **public** release

1. Install & run **`gitleaks`** or **`trufflehog`** — archive JSON report with reviewer initials.  
2. Choose **LICENSE / reuse** policy (`NOTICE-PRIVATE-COMPANION.md` placeholder superseded).  
3. Author-approved **visibility** decision + README rewrite for public readers.  
4. Verify **no future commits** introduce binaries / `.env` / operational dumps (**`.gitignore`** is not sufficient alone).  
5. Decide retail-book hyperlink strategy **after** companion posture firms up.  

---

## 11. Recommended release posture

| Flag | Assignment |
|------|-------------|
| **`KEEP_PRIVATE`** | **YES** *(current)* |
| **`INVITE_ONLY_READY`** | **PARTIAL** — infrastructure OK; **install leak scanners first** |
| **`PUBLIC_RELEASE_READY`** | **NO** — fails tooling + explicit author approval gates |

---

## 12. Change log *(this review artefact)*

Adds **`COMPANION-SECURITY-REVIEW.md`** only — **no** workbook content mutations.
