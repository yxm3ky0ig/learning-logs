# On-call notes — Aug 2026

## 2026-08-12 (Wed)

- **Incident:** Payment API timeout spike (15:30–16:10 JST)
- **Root cause:** DB connection pool exhaustion after deploy
- **Action:** Rolled back to previous version, raised pool size in config
- **Log:** See `logs/2026-08-12-payment-timeout.log`

## Takeaway

Always check connection pool metrics before scaling instances.
