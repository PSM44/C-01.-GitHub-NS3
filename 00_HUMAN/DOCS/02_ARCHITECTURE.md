# NS3 Architecture

## 1. Planes

| Plane | Responsibility | Prohibited responsibility |
|---|---|---|
| MORCH | objective boundary, material decisions, HUMAN status | inventing missing evidence |
| Control | identity, policy, routing, correlation, admission | accepting production output |
| RORCH | orchestration, DAG, retries, recovery | self-acceptance |
| Production | produces or repairs artifact | approval/custody |
| Quality | NTV, IV&V, deterministic oracles | production mutation |
| Veracity | compares claims against primary evidence | producing or accepting output |
| Security | policy, adversarial and negative testing | rewriting evidence |
| Custody | ledger, hashes, snapshots, verdict preservation | interpreting results |
| Evidence | durable references and provenance | operational dispatch authority |

## 2. Mandatory flow

`MORCH → Control → RORCH → Production → Quality/Veracity/Security → Custody → MORCH`

A rejection contains machine-readable findings and returns to RORCH. An acceptance is valid only after Custody records the corresponding evidence.

## 3. Communication rule

Every message must carry:
- protocol version;
- message, correlation and trace IDs;
- sender/recipient identities;
- timestamp and nonce hash;
- classification of permitted data;
- durable receipt or explicit fail-closed state.

## 4. Initial transport posture

Adapters are replaceable. Google Drive may provide evidence continuity; Slack may provide alerts; GitHub provides code/audit. None is accepted as a runtime command channel until the relevant adapter passes NS3 connectivity tests.
