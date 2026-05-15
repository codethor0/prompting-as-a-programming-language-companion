# STOP_CONDITIONS card

Examples—tailor per block:

- Missing authoritative identifier or timestamp on pasted evidence → halt with **`UNKNOWN`** rows.
- Tool requested outside **`ALLOWED_TOOLS`** → halt; propose narrower scope.
- Irreversible **`STATE_CHANGE`** without named reviewer → halt.
