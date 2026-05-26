# Agents Guide for `my-soc-ops-python`

## Mandatory development checklist

- `uv sync`
- `uv run ruff check .`
- `uv run pytest`

## What agents need to know

FastAPI + Jinja2 + HTMX workshop app.

Key entrypoints:
- `uv sync`
- `uv run pytest`
- `uv run uvicorn app.main:app --reload --host 0.0.0.0 --port 8000`

Core structure:
- `app/main.py`: routes
- `app/game_logic.py`: rule engine
- `app/game_service.py`: game state layer
- `app/models.py`: data schemas
- `app/data.py`: initial game data
- `app/static/`, `app/templates/`: UI

## Workflow

1. Read `README.md` and `pyproject.toml`.
2. Inspect `app/main.py`, templates, and tests.
3. Sync deps with `uv sync`.
4. Validate changes with `uv run pytest`.
5. Use a real browser, not VS Code Simple Browser.

## Notes

- Python `>=3.13`
- Lint with `ruff`
- Tests live in `tests/`
- Preserve the workshop flow and current app behavior

## Useful refs

- `.github/agents/`
- `.github/instructions/`
- `workshop/GUIDE.md`
