# JS Pain Demo

## Goal
Demonstrate:
- shared types between backend and frontend
- digest-pinned package manifest
- backend request/response flow
- frontend artifact generation
- request trace receipts

## Expected outputs
- `backend_summary.json`
- `frontend_build.json`
- `install_manifest.json`
- `request_trace.json`
- `summary.md`

## Required packages
- `web-core`
- `dom-core`
- `type-share-core`
- `install-core`
- `receipt-core`
- `report-core`

## Acceptance criteria
- same type contract is imported on both sides
- install manifest is digest-addressed
- at least one request flow is witnessed
- frontend artifact is reproducible
