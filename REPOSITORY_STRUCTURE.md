# NS3 Repository Information Architecture

## Canonical hierarchy

| Domain | Canonical function | Must not contain |
|---|---|---|
| 00_HUMAN | policy, definitions, unresolved decisions, use cases and approved documentation | runtime state, credentials or raw history |
| 01_SKILLS | reusable versioned internal and transversal methods | secrets or mutable run state |
| 02_IDEAS | proposals awaiting test and decision | implied commitments |
| 03_CONTINUITY | minimum non-derivable data needed to continue development in a new MORCH session or a completely blank AI | duplicate product truth or raw chat transcripts |
| 04_MEMORY | governed machine memory with scope, trust and expiry | authority to execute by itself |
| 05_MODELS | model-specific working data: operating profile, capabilities, configuration, compatibility and evaluations | provider credentials, private keys, unlicensed weights or unverified claims |
| 06_HARNESS | everything required to work with a named harness: setup, operation, integration, verification, rollback and known issues | credentials, mutable private databases or installed dependency trees |
| 09_RADAR | external signals and technology decision deltas | adoption by mere mention |
| 98_LEGACY | deprecated assets held for provenance/rollback | active canonical material |
| 99_IA.History | raw AI session provenance | normative instructions or current state |

## Required artefact conventions

1. Each document declares scope, authority, status, date and supersession.
2. Continuity stores only what a new MORCH or blank AI cannot safely derive from canonical sources; BATON is the entry package and HO1 is the reconstruction procedure.
3. A model or tool is not operational because it is installed or visible.
4. Every executable route has explicit identity, authorization, correlation, durable receipt, timeout and recovery policy.
5. Historical or legacy material is discoverable through an index and never silently treated as current.

## Pending structural additions

The current mandatory layout has no dedicated evidence or test domain. Before NS3 enables real payloads, decide whether to add:
- `07_EVIDENCE/`: immutable receipts, provenance, hashes and signed verdicts; and
- `08_TESTS/`: contract, adversarial, replay, fixture and recovery tests.

Until that decision, no claim may represent `99_IA.History`, `98_LEGACY` or `03_CONTINUITY` as evidence of a functional system.
