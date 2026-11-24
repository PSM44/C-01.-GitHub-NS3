# NS3 Repository Information Architecture

## Canonical hierarchy

| Domain | Canonical function | Must not contain |
|---|---|---|
| 00_HUMAN | policy, definitions, unresolved decisions, use cases and approved documentation | runtime state, credentials or raw history |
| 01_SKILLS | reusable versioned internal and transversal methods | secrets or mutable run state |
| 02_IDEAS | proposals awaiting test and decision | implied commitments |
| 03_CONTINUITY | recovery/transfer state references and orchestration handoff | duplicate product truth |
| 04_MEMORY | governed machine memory with scope, trust and expiry | authority to execute by itself |
| 05_MODELS | model manifests, routing and evaluation evidence | weights or provider credentials |
| 06_HARNESS | adapters, test contracts, qualification and rollback | untracked installed runtimes |
| 09_RADAR | external signals and technology decision deltas | adoption by mere mention |
| 98_LEGACY | deprecated assets held for provenance/rollback | active canonical material |
| 99_IA.History | raw AI session provenance | normative instructions or current state |

## Required artefact conventions

1. Each document declares scope, authority, status, date and supersession.
2. A continuity record points to canonical state; it must not replicate mutable truth.
3. A model or tool is not operational because it is installed or visible.
4. Every executable route has explicit identity, authorization, correlation, durable receipt, timeout and recovery policy.
5. Historical or legacy material is discoverable through an index and never silently treated as current.

## Pending structural additions

The current mandatory layout has no dedicated evidence or test domain. Before NS3 enables real payloads, decide whether to add:
- `07_EVIDENCE/`: immutable receipts, provenance, hashes and signed verdicts; and
- `08_TESTS/`: contract, adversarial, replay, fixture and recovery tests.

Until that decision, no claim may represent `99_IA.History`, `98_LEGACY` or `03_CONTINUITY` as evidence of a functional system.
