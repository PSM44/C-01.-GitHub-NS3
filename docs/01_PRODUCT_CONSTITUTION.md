# NS3 Product Constitution

## 1. Product purpose

NS3 is a system for executing an authorized engineering objective and determining whether its result deserves trust.

It resolves two coupled failures:
1. agent/runtime work loses authority, continuity, traceability, or recovery; and
2. the producer of an artifact can appear to validate its own work.

## 2. Non-negotiable invariant

A production component cannot accept, seal, or unilaterally declare its own output correct.

Acceptance requires evidence from the independent assurance and custody planes.

## 3. Functional boundary

NS3:
- receives an authorized objective through MORCH;
- plans and coordinates work through RORCH;
- produces an artifact;
- tests quality through NTV, IV&V, and deterministic oracles where applicable;
- contrasts claims with primary evidence;
- applies security policy and negative tests;
- preserves evidence and emits a verdict;
- recovers safely after interruption.

NS3 does not:
- treat installed software, a visible UI, or a model assertion as proof;
- enable a task merely because a message arrived;
- require HUMAN to relay prompts, artifacts, or receipts between components;
- make a material HUMAN decision automatically.

## 4. Authority

`HUMAN > MORCH > RORCH > EXE`

HUMAN receives material state and decisions from MORCH. RORCH and EXE do not use HUMAN as a transport channel.

## 5. Initial maturity claim

`PRODUCT_CONSTITUTION=PROPOSED_FOUNDATION`  
`RUNTIME_VALIDATION=NOT_PERFORMED`  
`SYSTEM_FUNCTIONAL=NOT_EVALUATED`
