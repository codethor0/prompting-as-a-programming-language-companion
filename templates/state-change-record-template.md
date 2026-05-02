# STATE_CHANGE record — template

## Purpose
Audit-ready note when persisted state differs after a workflow step.

## When to use
Databases, tickets, branching defaults, infra toggles, anything durable.

## Inputs
Baseline snapshot reference, actor IDs, approvals.

## Output artifact
Record block (**DRAFT — HUMAN_REVIEW_REQUIRED** until signed retention policy).

## Constraints
AI suggestions never apply **STATE_CHANGE** without human executor + approval artifact.

## Forbidden assumptions
“Helpful reorder” covertly mutates authoritative systems.

## Validation checks
- [ ] Planned vs observed diff enumerated  
- [ ] Rollback plan noted  

## STOP_CONDITIONS
Missing approver ⇒ no change.

## Human review
Mandatory signatory named.

## Version notes
Linkage to change ticket  

## QUESTIONS_FOR_OWNER
Retention duration uncertainty  
