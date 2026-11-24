# NS3 Data Classification

## Classes

| Class | Examples | May traverse PH-03 canary? | Storage rule |
|---|---|---:|---|
| C0 Public | public product metadata | yes | versioned repository allowed |
| C1 Internal | non-sensitive status, topology IDs | yes, if minimized | versioned with owner |
| C2 Controlled | work fixtures, findings, internal route details | no | restricted by policy and retention |
| C3 Sensitive | credentials, tokens, personal data, proprietary inputs | no | never commit; approved secret/data store only |
| C4 Custody | hashes, signed receipts, evidence snapshots and verdict references | metadata only | append-oriented, immutable or tamper-evident store |

## PH-03 canary allowlist

Only: nonce, timestamp, identity, status, protocol version, correlation ID, trace ID and nonce hash.

Any other field: `CANARY=REJECT`.

## Current status

`DATA_CLASSIFICATION=PROPOSED_FOUNDATION`  
`REAL_PAYLOADS=NOT_AUTHORIZED`
