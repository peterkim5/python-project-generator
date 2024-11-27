# Python Project Generator

A streamlined CLI tool for generating modern Python projects with best practices built-in.

## Features

- Creates a standardized Python project structure
- Sets up modern `pyproject.toml`-based configuration
- Initializes virtual environment with essential dev tools
- Supports both standard venv and `uv` for dependency management
- Generates basic module structure with example code
- Creates initial test setup with pytest
- Initializes git repository automatically

## Installation

1. Clone this repository:
```bash
git clone https://github.com/peterkim5/python-project-generator.git
cd python-project-generator
```

2. Make the script executable:
```bash
chmod +x create_project
```

3. (Optional) Add to your PATH for system-wide access:
```bash
# Add to your ~/.bashrc or ~/.zshrc:
export PATH="$PATH:/path/to/python-project-generator"
```

## Usage

```bash
./create_project my-new-project
```

This will create a new Python project with the following structure:
```
my-new-project/
├── src/
│   └── my_new_project/
│       ├── __init__.py
│       └── example.py
├── tests/
│   └── test_example.py
├── docs/
├── pyproject.toml
├── README.md
├── .gitignore
└── .venv/
```

## Configuration

The script supports the following environment variables:
- `PYTHON_CMD`: Python command to use (default: python3)
- `MINIMUM_PYTHON_VERSION`: Minimum Python version required (default: 3.10)
- `VERBOSE`: Enable verbose logging (set to 1)

## Requirements

- Python 3.10 or higher
- git (optional, but recommended)
- uv (optional, falls back to standard venv)

## License

MIT License - see LICENSE file for details

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.
