# llm-pocket

Minimal LLM CLI: stdin in, streamed answer out

## How to use

```bash
chatsh explain this error < error.log
cat diff.patch | chatsh review this diff
```

## Installation

```bash
pip install -r requirements.txt
export OPENAI_API_KEY=sk-...
```

## Highlights

- Model and system prompt via flags or env
- Streams tokens as they arrive
- Works with any OpenAI-compatible endpoint
- Reads the prompt from args or stdin

## Project structure

```text
├── .github/
│   └── pull_request_template.md
├── docs/
│   └── usage.md
├── examples/
│   └── quickstart.md
├── tests/
│   └── test_smoke.py
├── .gitignore
├── CHANGELOG.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── chatsh.py
└── requirements.txt
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
