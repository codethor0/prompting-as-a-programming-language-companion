# STOP_CONDITIONS — template

## Purpose
Explicit halts so enthusiasm does not ship missing evidence.

## When to use
Any workflow where missing context could cause harm, misinformation, or policy breach.

## Inputs
Policies, data-class rules, authority map.

## Output artifact
Enumerated stops + triggers (**DRAFT — HUMAN_REVIEW_REQUIRED**).

## Constraints
Stops are mandatory — no override by model tone.

## Forbidden assumptions
That “probably fine” waives a stop.

## Validation checks
- [ ] Each stop names evidence required to resume  
- [ ] Resume path names human role  

## STOP_CONDITIONS
*(Meta: if you cannot define stops, stop designing automation.)*

## Human review
Who may acknowledge exception (default: no one without written policy).

## Version notes
Change log of stop definitions  

## QUESTIONS_FOR_OWNER
Edge cases ambiguous to operators  
