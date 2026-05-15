# Private until approved

**Update (2026-05-15):** Repository visibility is **PUBLIC** so readers who follow the book appendix link can open starter templates without GitHub org membership. **Draft-quality expectations below still apply** until you run the release checklist and tag a reviewed revision.

This companion repository holds **draft workbook material**.

## Do **not**, without explicit author approval

- ~~Change visibility to **public** or distribute the URL broadly~~ *(visibility is now **public** by author decision — still do **not** misrepresent draft content as “final courseware”)*  
- Add a **hyperlink to this repo** in **retail or storefront prose** (*e.g.* KDP book body) unless the destination is finalized and intentional *(the book appendix already links here — keep repo content aligned with that responsibility)*  
- Share invite links casually — treat drafts as unpublished supporting material  

## Before any public release (checklist cues)

Run a **leak-detection scan** (for example **`gitleaks`** or **`trufflehog`**) on the revision you intend to open. Resolve every finding — **no placeholders allowed** for leaked access material.

Run a **human red-team pass** hunting for pasted operational data (`*.log` dumps, Slack exports, screenshots, identifiable individuals beyond agreed fictional personas).

Verify **every example file** stays **clearly fictional** or **explicitly sanitized** — no anecdotes that resemble identifiable commercial relationships unless you deliberately anonymized them with written policy.

Confirm **no manuscript-only authoring TODO lanes** linger (for example scaffolding tags meant for publishers). This repo mirrors practice assets, **not** the book’s staging comments.

Freeze a **semver or date-stamped tag** documenting what reviewers signed off — do not relabel unfinished trees as GA.
