# agent-eval-lab

Tiny eval harness: run prompt cases, score, compare

Started as a weekend hack, grew on me.

## What it does

- Exit code usable as a CI gate
- Keyword scoring + latency per case
- Cases defined in plain JSON
- Swap in any agent function via one line

## Usage

```bash
python evals.py
# edit cases.json, point run() at your agent
```

## Install

```bash
# stdlib only, nothing to install
```

## Project structure

```text
├── .github/
│   ├── ISSUE_TEMPLATE/
│   │   └── bug_report.md
│   └── dependabot.yml
├── docs/
│   ├── development.md
│   ├── roadmap.md
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .editorconfig
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── Makefile
├── cases.json
└── evals.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## FAQ

**Is this production ready?**  
It works for my use case; review the code before relying on it.

**Why no framework?**  
The stdlib covers what this project needs.

## License

MIT. Do whatever you want.
