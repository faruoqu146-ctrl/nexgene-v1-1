# NexGene v1.1.0

Phase 4: personalization context and the Weekly NexGene Report, building on Signals and security hardening.

## Run locally

```bash
docker compose up --build
```

Open **http://localhost:8000**.

## Test

```bash
docker compose exec api pytest -q
```

All 11 tests pass after fixes for datetime awareness (SQLite), valid dummy PBKDF2 hash, rate-limit isolation in tests, and contract version 1.1.0.

## v1.0.0 / v1.1.0 features

- Lightweight personal-context profile
- Weekly NexGene Report
- Signals
- Google Sign-In (optional)
- Optional AI-assisted reports
- Strong security posture (CSRF, rate limits, PBKDF2 600k, session revocation, etc.)
