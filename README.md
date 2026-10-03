# Analytics Event Schema Validator

Checks event schema declarations for identity, version, and privacy fields.

## How it works

`agent.py` applies the explicit rules in `RULES`, returns each failed rule with observed evidence and a review action, and derives status from the findings. It is deterministic, local-only, and uses no network or credentials.

## Run

```bash
python3 agent.py examples/good-input.json
python3 tools/audit-analytics-event-schema-validator.py examples/good-input.json
```

## Limitations

Uses caller-declared evidence only; it cannot establish that a real-world process is complete or compliant. Human review remains required.
