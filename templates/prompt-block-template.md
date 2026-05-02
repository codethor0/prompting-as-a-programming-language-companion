# Prompt block — template

## Purpose
Single reusable unit of intent with explicit boundaries for a language-model run.

## When to use
You have a recurring subtask that deserves a named handoff package.

## Inputs
- **Trusted context** (what reviewers already accept)  
- **Untrusted context** (anything that must never be treated as fact)  
- **Required fields** (…)  
- **Optional fields** (…)  

## Output artifact
Structured response following the declared output shape (**DRAFT — HUMAN_REVIEW_REQUIRED** until a human signs it for your real process).

## Constraints
- No invented facts for missing details — use **`UNKNOWN`**  
- No silent scope expansion  

## Forbidden assumptions
- That the model recalls prior chat  
- That probabilistic text equals tested code  

## Validation checks
- [ ] Output cites which inputs it relied on  
- [ ] Contradictions flagged, not smoothed over  

## STOP_CONDITIONS
- Halt if required inputs missing or policy forbids processing  

## Human review
Named approver before any **STATE_CHANGE**, send, publish, or customer-facing use.

## Version notes
Revision ID · date · what changed  

## QUESTIONS_FOR_OWNER
- List open questions the model must not guess  
