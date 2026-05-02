# Data analysis workflow *(draft template)*

**status:** draft template  

## Fictional / sanitized data notice
Coffee shop KPIs fabricated for **Harbor Trail Coffee**—not benchmark truth.

## Workflow goal
Move from question → sanitized table spec → plotted narrative (**DRAFT — HUMAN_REVIEW_REQUIRED**).

## Primary inputs
Question, metric definitions (**fictional**).

## Supporting context
Prior agreed schema version.

## Prompt blocks
`BLOCKclarifyQ`, `BLOCKplanSQLorSheet`, `BLOCKinterpret` (interpretation barred from asserting causality).

## Handoffs
Each step outputs validation gates + STOP hooks.

## Tool permissions
Runtime tools **outside** companion — declare **none** by default internally.

## State changes
Publishing dashboards ⇒ human **STATE_CHANGE** first.

## Validation
Integrity checks enumerated; outliers flagged **`UNKNOWN`** if cause unclear.

## STOP_CONDITIONS
Stop if aggregated data approximates real persons’ purchase trails.

## Final artifact
**DRAFT — HUMAN_REVIEW_REQUIRED** analytic brief skeleton.

## QUESTIONS_FOR_OWNER
Statistical framing beyond operator skill? escalate.  
