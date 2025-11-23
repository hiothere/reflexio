# Reflexio

Composable retry policies with pluggable classifiers, per-class backoff, and structured hooks.

## Quick start

```python
from reflexio import retry

@retry  # uses default_classifier + decorrelated_jitter(max_s=5.0)
def fetch_user():
    ...
```

Async uses the same decorator, or `AsyncRetryPolicy` directly.

## What’s inside

- [Usage](usage.md) – policies, decorators, strategies, deadlines, hooks.
- [Observability](observability.md) – metric/log hook contracts and patterns.
- [Recipes](recipes.md) – HTTPX, async workers, pyodbc SQLSTATE classifier, FastAPI proxy.
- Snippets in `docs/snippets/` back the recipes and can be run with `uv run ...`.
