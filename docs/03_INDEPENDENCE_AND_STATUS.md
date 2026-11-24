# NS3 Independence and Status Contract

## 1. Independence grades

| Grade | Separation | Acceptance use |
|---|---|---|
| G0 | same process/context | not independent |
| G1 | role or prompt only | advisory only |
| G2 | process, context and queue separated | basic operational isolation |
| G3 | separate runtime identity, permissions and evidence path | minimum QA/veracity/security independence |
| G4 | separate VM/host, identity, custody store and administrative boundary | custody and critical security |

Minimum targets:
- Production vs Quality: G3
- Production vs Veracity: G3
- Production vs Security: G3
- Custody: G4

A second prompt to the same model is G1, not an independent audit.

## 2. HUMAN-visible status

MORCH must make these fields available:
- `NS3_STATE=OPERATIONAL|DEGRADED|BLOCKED|RECOVERING|UNKNOWN`
- `LAST_END_TO_END_PASS`
- `ACTIVE_RUN`
- `SECTOR_HEALTH`
- `INDEPENDENCE_GRADE`
- `LAST_FAILURE`
- `RECOVERY_STATE`
- `HUMAN_ACTION_REQUIRED`
- `EVIDENCE_REFERENCE`

No fresh heartbeat or no durable evidence produces `NS3_STATE=UNKNOWN`, not an implicit healthy state.

## 3. Alert policy

- OPERATIONAL: visible on demand.
- DEGRADED: MORCH receives cause and automatic recovery state.
- BLOCKED: HUMAN receives only the material decision or blocker.
- UNKNOWN: immediate visible warning; no PASS claim is allowed.
