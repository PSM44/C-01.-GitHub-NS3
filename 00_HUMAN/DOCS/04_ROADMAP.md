# NS3 Roadmap v0.1

## NS3-PH-00 — Foundation contract
Deliverables: product constitution, topology registry, threat model, data classification, authority contract.
Exit: each sector, required edge, identity and independence target is defined.

## NS3-PH-01 — Internal communication fabric
Deliverables: envelope, identity/policy gate, durable inbox/outbox, ledger, route controller, health doctor, MORCH status contract.
Exit: all components can be discovered and their health is explicit.

## NS3-PH-02 — Links and negative controls
Deliverables: adapters for MORCH, RORCH, production, quality, veracity, security and custody.
Exit: allowed links are authenticated; forbidden links are rejected and evidenced.

## NS3-PH-03 — Connectivity-only canary
Permitted data: nonce, IDs, identities, timestamps, statuses and nonce hashes only.
Exit: every mandatory edge has a bilateral correlated receipt, durable ledger record, freshness proof and replay rejection.
Required state:
```
HAAPI_ELIMINATION=PASS
NETWORK_INTERNAL=PASS
ALL_REQUIRED_EDGES=BIDIRECTIONAL_VERIFIED
HUMAN_STATUS_VISIBILITY=PASS
SYSTEM_FUNCTIONAL=NOT_EVALUATED
```

## NS3-PH-04 — Synthetic transfer and independence canary
Deliverables: controlled fixture, defect-seeded fixture, recovery drill.
Exit: quality, veracity and security independently detect designated failures; custody remains G4.

## NS3-PH-05 — Closed product cycle
Deliverables: production-to-assurance-to-custody-to-rework cycle.
Exit: correct fixture accepted, defective fixture rejected, rework is correlated, evidence is sealed.

## NS3-PH-06 — First bounded real task
Gate: separately authorized.
Exit: real task completes without HUMAN relay, with rollback and final evidence.

## Constraints

No production claim is allowed from package presence, UI visibility, mocked data, one-way receipt, stale heartbeat, or a shared producer/auditor context.
