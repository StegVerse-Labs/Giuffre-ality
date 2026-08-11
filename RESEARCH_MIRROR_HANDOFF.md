# Giuffre-ality Research Mirror Handoff

## Authority
- goal_id: ERL-RESEARCH-SURFACE-GIUFFRE-001
- repository: StegVerse-Labs/Giuffre-ality
- branch: main
- canonical_owner: StegVerse-Labs/Executive_Rhetoric_Ledger Issue #60
- local_role: subject-specific biography/event/location/story source discovery and candidate production
- evaluation_authority: StegVerse-Labs/Executive_Rhetoric_Ledger
- credential_authority: TV/TVC where applicable
- github_token_authority: NONE

## Claim
- state: CLAIMED_FOR_VALIDATION
- release_condition: deterministic populated fixture + ERL intake validation + registry promotion

## Installed authoritative files
`research/README.md`, `research/frontier.json`, `research/acquisition_requests.jsonl`, `research/source_candidates.jsonl`, `research/research_receipts.jsonl`, `research/conformance.json`, `data/sources/sources_whitelist.csv`, `scripts/search_agent.py`.

Upstream standard: `StegVerse-Labs/Executive_Rhetoric_Ledger/standards/multi-trajectory-research-surface.v1.md`.
Upstream transport: `StegVerse-Labs/Executive_Rhetoric_Ledger/contracts/research-candidate-transport.v1.md`.

## Research posture
- recurrence: REQUIRED while documentary, memoir, court, institutional, or public-record evidence can alter OPEN/ACTIVE trajectories;
- default cadence: weekly, adjusted by trajectory volatility;
- `.github/workflows/weekly-ingest.yml` is transport/ingest, not automatically a research monitor;
- contradictory/null/new trajectories are preserved; local output remains lead-only/context-only until ERL review.

## Evidence
- research surface: `c35983e12ff5c9d4d6c4a712af0973ace966fab1`
- conformance profile: `ae6830713a0285fa9da653071f8becdebadaf292`
- adapter transport alignment: `4afa3f21518f84907eb8f7acd163328ad70908d2`

The adapter now emits the ERL candidate v1 schema with full repository identity, no native/evaluation mutation, TV/TVC credential authority, GitHub token authority NONE, and authority effect NONE.

## Remaining
1. deterministic populated fixture and adapter execution proof;
2. ERL candidate intake validation;
3. registry promotion to CONFORMING.

## Validation
- `python scripts/search_agent.py --base . --dry-run`
- `python <ERL>/scripts/validate_research_surface.py .`
- `python <ERL>/scripts/validate_research_candidate_intake.py research/source_candidates.jsonl`

## Completion accounting
- developed-files: 9/9 = 100%
- scaffolding/stubs: 0
- validation: 0/3
- integration: 2/3
- goal-activation: 75%
