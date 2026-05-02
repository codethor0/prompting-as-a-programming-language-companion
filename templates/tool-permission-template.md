# Tool permission — template

## Purpose
Least-privilege ledger for tooling calls surfaced to a model-mediated workflow.

## When to use
Before enabling read/write integrations.

## Inputs
Threat model slice, sensitivity classes, outage contacts.

## Output artifact
Permission matrix (**DRAFT — HUMAN_REVIEW_REQUIRED**).

## Constraints
Default: **none** granted until explicitly listed with scope + expiry posture.

## Forbidden assumptions
Read-only tools cannot influence downstream harm paths.

## Validation checks
- [ ] Each capability tied to reversible preview path  
- [ ] Logging destination named  

## STOP_CONDITIONS
Stop if tooling scope creep detected mid-session.

## Human review
Approve expansions beyond read-only exploratory sandboxes.

## Version notes  
Matrix revision  

## QUESTIONS_FOR_OWNER
Ambiguous SaaS IAM boundaries  
