# greet-ci

A simple greeting program with GitHub Actions CI.

## Setup

```bash
uv lock
```

## Usage

```bash
uv run --locked python greet.py Hee   # Hello, Hee!
uv run --locked python greet.py       # Hello, world!
```

## Local checks

```bash
uv run --locked pytest -q greet.py
uv run --locked black --check greet.py
uv run --locked flake8 greet.py
uv run --locked mypy greet.py
uv build
```
