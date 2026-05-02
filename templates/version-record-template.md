# Version record — template

## Purpose
Treat prompts like versioned artefacts: who changed what, why, deltas.

## When to use
Any block/chain slated for repetition or regression testing.

## Inputs
Prior revision hash or label, reviewer list.

## Output artifact
Changelog snippet (**DRAFT — HUMAN_REVIEW_REQUIRED** if affects production lane).

## Constraints
 semver / date / human label — pick one convention and stick to it.

## Forbidden assumptions
Silent overwrites erase accountability.

## Validation checks
- [ ] Diff summary human-readable  
- [ ] Automated tests/manual checks referenced  

## STOP_CONDITIONS
Stop if divergence rationale undocumented.

## Human review
Approver for semver bump tiers you define locally.

## Version notes
Embedded in header of this template instance  

## QUESTIONS_FOR_OWNER
Branching vs linear history preference  
