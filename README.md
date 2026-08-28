# quillstatic-app

Static blog generator: markdown in, tidy HTML out

Side project, maintained when I have time.

## How to use

```bash
mkdir posts && echo '# hello' > posts/first.md
python build.py
# site lands in dist/
```

## Install

```bash
pip install -r requirements.txt
```

## What it does

- RSS feed generation
- Index page with post list by date
- Single template, plain str.format, no Jinja
- Markdown posts with fenced code and tables

## Project structure

```text
├── .github/
│   ├── dependabot.yml
│   └── pull_request_template.md
├── docs/
│   ├── roadmap.md
│   └── usage.md
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── Makefile
├── SECURITY.md
├── build.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## License

MIT - see [LICENSE](LICENSE).
