# NS3 Topology Registry

## 1. Required sectors

| ID | Sector | Role | Required independence |
|---|---|---|---|
| S1 | HUMAN | material decisions and visibility | external authority |
| S2 | MORCH | orchestration boundary and status | control identity |
| S3 | Control Plane | identity, policy, routing, ledger admission | separate from producer |
| S4 | RORCH | task orchestration and recovery | separate context |
| S5 | Production | artifact production or repair | cannot accept itself |
| S6 | Quality / NTV / IV&V | deterministic and evaluative verification | G3 |
| S7 | Veracity | claim-to-primary-evidence comparison | G3 |
| S8 | Security | policy and adversarial/negative checks | G3 |
| S9 | Custody | evidence preservation and verdict reference | G4 |

## 2. Mandatory edges

| Edge | Direction | Initial permitted payload | Pass condition |
|---|---|---|---|
| E1 | MORCH ↔ Control | control-plane canary only | bilateral correlated receipts |
| E2 | Control ↔ RORCH | control-plane canary only | policy-authenticated route |
| E3 | RORCH ↔ Production | control-plane canary only | replay-safe bilateral route |
| E4 | Production ↔ Quality | fixture only after PH-03 | independent receipt and verdict |
| E5 | Production ↔ Veracity | fixture only after PH-03 | independent comparison receipt |
| E6 | Production ↔ Security | fixture only after PH-03 | negative-control receipt |
| E7 | Assurance ↔ Custody | evidence metadata only | immutable evidence reference |
| E8 | Custody → MORCH | status/verdict reference only | durable correlated state |

No edge is operational because a UI, package, VM or account exists.

## 3. Current status

`TOPOLOGY=DEFINED_NOT_CONNECTED`  
`MANDATORY_EDGES_VERIFIED=0/8`
