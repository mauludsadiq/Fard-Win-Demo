# Control Tower

## Goal
Collect and verify outputs from:
- `py_pain_demo`
- `rust_pain_demo`
- `js_pain_demo`

## Outputs
- `summary.json`
- `summary.md`
- `benchmark_table.json`
- `replay_checks.json`
- `receipts/`

## Acceptance criteria
- every reported win is tied to an artifact
- every artifact has a digest
- replayable stages are checked
- benchmark table is rendered
