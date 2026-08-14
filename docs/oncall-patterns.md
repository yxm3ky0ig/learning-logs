# On-Call Patterns

Quick notes from recent incidents.

## 2026-08-13
- DB connection pool exhaustion: raised max connections, added retry with backoff.
- Silent alert fatigue: reviewed thresholds, adjusted paging rules for non-critical.

## Pattern
- Always check recent deploys before deep diving.
- Log timestamps in UTC to avoid confusion.
