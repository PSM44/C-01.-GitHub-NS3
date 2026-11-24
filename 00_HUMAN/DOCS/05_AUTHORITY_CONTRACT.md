# NS3 Authority Contract

## 1. Authority chain

`HUMAN → MORCH → RORCH → EXECUTION`

| Role | May do | Must not do |
|---|---|---|
| HUMAN | authorize scope, material risk, real-world impact and irreversible decisions | relay routine system messages |
| MORCH | expose status, maintain objective boundary, request material decisions, terminate unsafe work | fabricate missing evidence or accept production output |
| RORCH | decompose authorized work, schedule routes, coordinate rework and recovery | broaden scope or accept its own production |
| EXECUTION | perform an approved bounded action | self-approve, seal evidence or change authority |
| Assurance | test, verify and reject according to policy | alter production output |
| Custody | preserve receipts, hashes, snapshots and verdict references | reinterpret or edit findings |

## 2. Admission rule

An execution request is admitted only when it has:
- an authorized objective and scope;
- sender and recipient identities;
- policy decision;
- correlation and trace identifiers;
- permitted data classification;
- timeout, rollback or recovery route;
- durable receipt.

Otherwise: `ADMISSION=DENY`.

## 3. Material decision boundary

Only HUMAN may authorize:
- irreversible external actions;
- credential creation or rotation;
- paid-resource commitment;
- access-scope expansion;
- model or harness adoption for production;
- real payload activation after the canary phases.

## 4. Current status

`AUTHORITY_CONTRACT=PROPOSED_FOUNDATION`  
`EXECUTION_ADMISSION=NOT_IMPLEMENTED`
