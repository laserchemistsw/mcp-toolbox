# mcp-toolbox

MCP server template I base new tools on

Started as a weekend hack, grew on me.

## Usage

```bash
# claude_desktop_config.json
# {
#   "mcpServers": {
#     "notes-box": {"command": "python", "args": ["server.py"]}
#   }
# }
python server.py
```

## What it does

- State persisted to a JSON file in the home dir
- Includes Claude Desktop config snippet
- FastMCP style: decorators, zero boilerplate
- Three tools: add / get / list notes

## Installation

```bash
pip install -r requirements.txt
```

## Project structure

```text
├── .github/
│   └── dependabot.yml
├── docs/
│   ├── faq.md
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
├── SECURITY.md
├── requirements.txt
└── server.py
```

## Development

```bash
python -m venv .venv && source .venv/bin/activate
pip install -r requirements.txt
python -m pytest -q
```

## Why

Needed this for myself; figured others might too.

## License

MIT licensed, see LICENSE.
