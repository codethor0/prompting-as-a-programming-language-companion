# Agent-loop workflow *(draft template — bounded)*

**status:** draft template  

## Fictional / sanitized data notice
Exercise uses synthetic goals only.

## Workflow goal
Illustrate goal → bounded tool → observation → validator → escalate loop with strict ceilings.

## Primary inputs
Loop objective (**fiction**), max cycles integer (small).

## Supporting context
Pre-approved tool manifest (possibly empty).

## Prompt blocks integrated as loop body
Planner micro-block, Executor micro-block, Critic micro-block — each **DRAFT — HUMAN_REVIEW_REQUIRED** at exit unless marked internal scratch only.

## Handoffs
State vector serialized textually (**no live DB IDs**).

## Tool permissions
**Default: none** — explicit allowlist enumerates harmless read sandboxes **you** maintain.

## State changes
Forbidden without human console operator.

## Validation
Invariant checks enumerated per iteration.

## STOP_CONDITIONS
Cycle budget exceeded ⇒ STOP cold.

## Final artifact
**DRAFT — HUMAN_REVIEW_REQUIRED** loop transcript excerpt.

## QUESTIONS_FOR_OWNER
Residual autonomy creep risks if critic silenced—who re-enables critic? **`UNKNOWN`** until named.  
