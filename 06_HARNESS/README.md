# Harness

Everything needed to work with a harness technology, such as DeepSeek Harness (DSH), Hermes Harness, OpenClaw2 or a future equivalent.

Each harness domain may contain installation and update procedures, operating modes, workspace policies, launcher contracts, integrations, connectors, compatibility matrices, verification procedures, rollback/recovery, known defects and harness-specific documentation.

Recommended pattern:

```
06_HARNESS/
└── DSH/
    ├── README.md
    ├── installation.md
    ├── configuration.md
    ├── operating-modes.md
    ├── integrations.md
    ├── verification.md
    ├── rollback.md
    └── known-issues.md
```

Harness source material and approved runbooks may be versioned. Credentials, personal tokens, mutable private runtime databases and installed dependency trees are excluded.
