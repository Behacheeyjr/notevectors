# notevectors

Semantic search over local notes with embeddings

## Highlights

- Reranks by recency when scores tie
- Vectors cached to .npy so re-runs are instant
- Interactive REPL and one-shot modes
- sentence-transformers when available, TF-IDF fallback

## Examples

```bash
python search.py ./notes
>> how do I back up my database?
```

## Getting started

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── workflows/
│       └── ci.yml
├── docs/
│   ├── development.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── SECURITY.md
├── requirements.txt
└── search.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```
