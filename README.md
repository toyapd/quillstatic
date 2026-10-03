# quillstatic

Static blog generator: markdown in, tidy HTML out

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

- Single template, plain str.format, no Jinja
- Index page with post list by date
- RSS feed generation
- Markdown posts with fenced code and tables

## Project structure

```text
├── .github/
│   └── workflows/
│       └── ci.yml
├── .gitignore
├── CHANGELOG.md
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── SECURITY.md
├── build.py
└── requirements.txt
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
```

## FAQ

**Is this production ready?**  
It works for my use case; review the code before relying on it.

**Why no framework?**  
The stdlib covers what this project needs.

## License

MIT licensed, see LICENSE.
