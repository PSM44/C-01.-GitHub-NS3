# NS3 Initial Threat Model

## Threats and mandatory controls

| Threat | Failure | Mandatory control | Evidence required |
|---|---|---|---|
| Spoofed sender | forged authority | workload identity and policy gate | authenticated receipt |
| Replay | duplicate or stale execution | nonce, expiry, idempotency and ledger | replay rejection |
| Misroute | data/action reaches wrong sector | recipient binding and classification check | policy denial |
| Self-approval | producer accepts its own output | G3 assurance/veracity/security separation; G4 custody | independent correlated verdict |
| Silent failure | component dies without visibility | heartbeat, expiry and `UNKNOWN` status | stale-state transition |
| Evidence tampering | receipt/finding altered | hash, append-only record and custody boundary | integrity verification |
| Privilege escalation | component gains unapproved capability | least privilege and explicit HUMAN approval | denied escalation record |
| Human relay regression | HUMAN becomes transport again | machine-to-machine route and MORCH-only status | end-to-end route evidence |

## Explicit non-claims

This model is a design baseline. It is not a penetration test, a runtime security assessment or proof that any control is operating.

`THREAT_MODEL=PROPOSED_FOUNDATION`  
`SECURITY_VALIDATION=NOT_PERFORMED`
