# Package Contracts

## `receipt-core`
Responsible for:
- canonical receipt construction
- digest derivation
- parent/child chaining
- artifact reference representation

Must expose:
- `receipt.mk(parts)`
- `receipt.digest(receipt)`
- `receipt.chain(parent, payload_digest)`

## `replay-core`
Responsible for:
- snapshot digest verification
- replay comparison
- mismatch diagnostics

Must expose:
- `replay.verify(receipt, snapshot)`
- `replay.compare(a, b)`

## `report-core`
Responsible for:
- summary rendering
- markdown and json report emission
- benchmark table rendering

## `bench-core`
Responsible for:
- timing capture
- memory capture where possible
- benchmark record normalization

## `dataframe-core`
Responsible for:
- ingest
- filter
- project
- group_by
- aggregate
- sort
- schema introspection
- deterministic output digests

## `plot-core`
Responsible for:
- histogram
- bar chart
- line chart
- artifact emission
- digesting rendered output

## `ml-core`
Responsible for:
- model state
- training loop
- checkpoint CID generation
- result summaries

## `serve-core`
Responsible for:
- local serve interface
- route handling
- JSON/text response output
- request/response receipt generation

## `par-core`
Responsible for:
- parallel map
- parallel filter
- parallel reduce
- deterministic reduction output rules

## `json-core`
Responsible for:
- parse throughput benchmark surfaces
- deterministic parse representation
- aggregate helpers

## `web-core`
Responsible for:
- backend app surface
- typed request/response handling
- route registration

## `dom-core`
Responsible for:
- render tree creation
- static render or bundle artifact emission
- digestable build artifacts

## `type-share-core`
Responsible for:
- shared type import/export discipline
- consistent schema use across frontend and backend

## `install-core`
Responsible for:
- digest-pinned install manifest generation
- package lock representation
- install report output
