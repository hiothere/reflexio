# Examples

- HTTPX sync: `uv pip install httpx` then `uv run python docs/snippets/httpx_sync_retry.py`
- HTTPX async: `uv pip install httpx` then `uv run python docs/snippets/httpx_async_retry.py`
- requests sync: `uv pip install requests` then `uv run python docs/snippets/requests_retry.py`
- Async worker loop: `uv run python docs/snippets/async_worker_retry.py`
- Decorator basics: `uv run python docs/snippets/decorator_retry.py`
- FastAPI proxy with retries: `uv pip install "fastapi[standard]" httpx` then `uv run uvicorn docs.snippets.fastapi_downstream:app --reload`
- FastAPI middleware with per-endpoint policies: `uv pip install "fastapi[standard]" httpx` then `uv run uvicorn docs.snippets.fastapi_middleware:app --reload`
- PyODBC + SQLSTATE: `uv pip install pyodbc` then `uv run python docs/snippets/pyodbc_retry.py`
- asyncpg + SQLSTATE: `uv pip install asyncpg` and set `ASYNC_PG_DSN`, then `uv run python docs/snippets/asyncpg_retry.py`
- Benchmarks (pyperf): `uv pip install .[dev]` then `uv run python docs/snippets/bench_retry.py`
