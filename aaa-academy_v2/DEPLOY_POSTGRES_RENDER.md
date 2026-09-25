# AAA Academy — Render + PostgreSQL

## Render Web Service

Build:
```bash
pip install -r requirements.txt
```

Start:
```bash
uvicorn app.main:app --host 0.0.0.0 --port $PORT
```

## Environment variable

Add this in Render:
```text
DATABASE_URL=<Render PostgreSQL Internal Database URL>
```

Do not commit database passwords or DATABASE_URL to GitHub.

## Important

The legacy `aaa_academy.db` is retained in this archive for migration/reference.
It should not be used as the production database once DATABASE_URL is configured.
