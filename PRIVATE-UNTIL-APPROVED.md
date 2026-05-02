# Private until approved

This companion repository holds **draft workbook material**.

## Do **not**, without explicit author approval

- Change visibility to **public** or distribute the URL broadly  
- Add a **hyperlink to this repo** in **retail or storefront prose** (*e.g.* KDP book body) unless the destination is finalized and intentional  
- Share invite links casually — treat drafts as unpublished supporting material  

## Before any public release (checklist cues)

Run a **leak-detection scan** (for example **`gitleaks`** or **`trufflehog`**) on the revision you intend to open. Resolve every finding — **no placeholders allowed** for leaked access material.

Run a **human red-team pass** hunting for pasted operational data (`*.log` dumps, Slack exports, screenshots, identifiable individuals beyond agreed fictional personas).

Verify **every example file** stays **clearly fictional** or **explicitly sanitized** — no anecdotes that resemble identifiable commercial relationships unless you deliberately anonymized them with written policy.

Confirm **no manuscript-only authoring TODO lanes** linger (for example scaffolding tags meant for publishers). This repo mirrors practice assets, **not** the book’s staging comments.

Freeze a **semver or date-stamped tag** documenting what reviewers signed off — do not relabel unfinished trees as GA.
