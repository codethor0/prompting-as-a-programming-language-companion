# Agent-loop spec — template *(bounded automation)*

## Purpose
Declare a **tight loop** — goal → act → observe → validate — with hard gates, not autonomy theatre.

## When to use
You need repeatable multi-step autonomy under explicit ceilings.

## Inputs
Objective, environment map, allowable tools (**default none** unless listed).

## Output artifact
Spec doc (**DRAFT — HUMAN_REVIEW_REQUIRED**).

## Constraints
 Loop cannot broaden mission, grant tools, or alter records without escalated human approvals.

## Forbidden assumptions
“Agent” label implies correctness or authority.

## Validation checks
- [ ] Cycle budget enumerated  
- [ ] Escalation / STOP paths rehearsed  

## STOP_CONDITIONS
Any unknown risk class halts autonomous continuation.

## Human review
Mandatory before first production-adjacent run and after anomalies.

## Version notes  
Spec semver  

## QUESTIONS_FOR_OWNER
Residual autonomy debt when tools fail silently  
