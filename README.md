# Python Toolbox

A collection of small, reusable Python tools and utilities for everyday scripting, automation, and development.

The project should keep tools small, reusable, composable, and easy to test.

## Structure

```text
python-toolbox/
├── bin/             # Executable Python tools
├── src/
│   └── toolbox/     # Reusable Python modules
├── tests/           # pytest and unittest
├── docs/            # Documentation
├── pyproject.toml   # Project configuration
├── README.md
└── LICENSE
```

## Library

Reusable functionality lives under `src/toolbox/`.

```python
from toolbox.text import fields_after
```

Modules are organized by purpose rather than by application.

Examples:

```text
src/toolbox/
├── __init__.py
├── text.py
├── files.py
├── csv.py
├── json.py
└── shell.py
```

## Command-line Tools

Standalone tools live under `bin/`.

```text
bin/
├── csv-columns
├── json-format
└── file-info
```

The goal is to make individual tools useful from the command line while keeping their underlying functionality reusable from Python.

## Testing

Tests use both `pytest` and Python's standard-library `unittest` and live under `tests/`.

```bash
pytest
python -m unittest
```

## Development

Create a virtual environment:

```bash
python -m venv .venv
source .venv/bin/activate
```

Install the project in editable mode:

```bash
python -m pip install -e .
```

## Design Principles

* Small, focused utilities
* Reusable Python code
* Command-line friendly
* Minimal dependencies
* Standard library where practical
* Easy to test
* Composable tools
* Clear interfaces
* No unnecessary abstractions

A collection of small, reusable Python utilities for scripting, automation, and development. The package is distributed through PyPI and can be installed used across projects.

## Status

Currently under development.

## License

See [LICENSE](LICENSE).
