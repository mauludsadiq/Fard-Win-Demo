# Benchmark Targets

## Python-facing targets
- CSV ingest and analytics pipeline
- group-by throughput
- plot generation latency
- small-model training and checkpoint emission
- serve startup

## Rust-facing targets
- process startup
- JSON parse on a 10MB payload
- parallel map/filter/reduce
- memory footprint summary

## JS-facing targets
- backend route setup
- shared-type request flow
- frontend artifact generation
- install manifest digest emission

## Global reporting
Each benchmark record should include:
- `name`
- `cohort`
- `input_digest`
- `output_digest`
- `duration_ms`
- `notes`
- `receipt_digest`
- `replayable`
