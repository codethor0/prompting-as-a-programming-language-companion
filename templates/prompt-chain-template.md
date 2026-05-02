# Prompt chain — template

## Purpose
Ordered **prompt blocks** connected by validated handoffs.

## When to use
A task naturally splits into stages with receipts between stages.

## Inputs
Overall goal, staged inputs per block, escalation policy.

## Output artifact
Stack of staged outputs + validation notes ending in **DRAFT — HUMAN_REVIEW_REQUIRED** until signed.

## Constraints
Blocks run in declared order — no reordering without human approval.

## Forbidden assumptions
That intermediate prose is production-ready without stage checks.

## Validation checks
- [ ] Handoff package between stages complete  
- [ ] Each gate records pass/fail with evidence slices  

## STOP_CONDITIONS
Any stage may halt chain if evidence/policy gaps arise.

## Human review
Mandatory before merges to external-facing channels or persistence that matters.

## Version notes
Chain spec ID · changelog  

## QUESTIONS_FOR_OWNER
Ownership of ambiguous stages  
