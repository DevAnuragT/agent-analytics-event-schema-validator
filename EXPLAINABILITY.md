# Decision and Reasoning

Checks event schema declarations for identity, version, and privacy fields. Each rule is checked independently; all rules must pass for status `pass`.

# Inputs and Data Sources

Input is a caller-provided JSON object. No remote or private data is accessed.

# Known Limitations

Caller-provided evidence is not independently verified. The result is a bounded pre-review aid, not certification.
