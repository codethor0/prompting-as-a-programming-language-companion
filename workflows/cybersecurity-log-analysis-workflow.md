# Cybersecurity log analysis workflow *(draft template)*

**status:** draft template  

## Fictional / sanitized data notice
Synthetic lines only. No raw production logs pasted here—ever.

## Workflow goal
Triage fabricated alert bundles into timeline + hypotheses (**DRAFT — HUMAN_REVIEW_REQUIRED**).

## Primary inputs
Redacted excerpts, IOC table skeleton (empty ok).

## Supporting context
Runbook locator internal to operator org (**not reproduced**).

## Prompt blocks
`BLOCKinventory`, `BLOCKtimeline`, `BLOCKhypothesis` with explicit UNKNOWN separation.

## Handoffs
Each stage cites evidence lineage.

## Tool permissions
**Default: none** — analysis sandboxes segregated externally by you.

## State changes
Tickets / escalation paths require human—not model—submission.

## Validation
Facts vs guesses table mandatory.

## STOP_CONDITIONS
Real credential-like strings detected ⇒ immediate halt + rotate handling per **your** incident policy (not scripted here).

## Final artifact
**DRAFT — HUMAN_REVIEW_REQUIRED** investigative memo shell.

## QUESTIONS_FOR_OWNER
Authority to engage IR vendor? **`UNKNOWN`** until named.  
