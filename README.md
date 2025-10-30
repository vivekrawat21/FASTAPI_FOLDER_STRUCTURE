# FastAPI Project

A minimal, opinionated FastAPI project structure. This repository provides a small starting scaffold for building REST APIs with FastAPI.

## Quick start

1. Create and activate a virtual environment

```bash
python3 -m venv .venv
source .venv/bin/activate
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

3. Run the app

```bash
uvicorn app.main:app --reload --host 0.0.0.0 --port 8000
```

4. Open the docs

- Swagger UI: `http://127.0.0.1:8000/docs`
- ReDoc: `http://127.0.0.1:8000/redoc`

## Run tests

After installing dev/test dependencies in `requirements.txt`:

```bash
pytest -q
```

## Project layout (short)

- `app/main.py` - application factory and router registration
- `app/api/v1/` - versioned API (routes, schemas, controllers)
- `app/core/` - configuration (Pydantic settings)
- `app/database/` - database connection and models (placeholder)
- `app/services/` - business logic layer
- `app/tests/` - pytest tests
- `requirements.txt` - project dependencies

## Environment

Copy `.env.example` to `.env` and edit as required.

## Contributing

Contributions are welcome. Please open issues or pull requests with focused changes.
