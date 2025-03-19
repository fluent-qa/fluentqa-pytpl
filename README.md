# README

This project is a template UV project

- create project by UV, because UV is so fast

```
As a python Beginer, use UV to management Python Dev evnironment, key points for basic usage:

- How to use uv to create a virtual environment with different python version

- How to use uv to add/remove python packages

- How to use uv to Build/Run python project

- How to use uv to manage different scripts like package.json in Node.js

Please replay as simple as possible in markdown format, and use code block to show the commands, please make sure as simple as possible, and one question then another.

Don't explain too much, just focus on how to use uv to manage a python project without any advanced knowledge or skill.
```

# UV for Python Beginners

## Creating a Virtual Environment

Create a virtual environment with the default Python version:

```bash
uv venv .venv
```

Create with a specific Python version:

```bash
uv venv .venv --python=3.10
```

Activate the environment:

```bash
source .venv/bin/activate
```

## Managing Python Packages

Add packages:

```bash
uv pip install requests
```

Add multiple packages:

```bash
uv pip install requests pandas matplotlib
```

Add with specific version:

```bash
uv pip install requests==2.31.0
```

Remove packages:

```bash
uv pip uninstall requests
```

List installed packages:

```bash
uv pip list
```

## Building/Running Python Projects

Run a Python script:

```bash
uv python script.py
```

Install project dependencies from requirements.txt:

```bash
uv pip install -r requirements.txt
```

## Managing Scripts (like package.json)

Create a pyproject.toml file:

```toml
[tool.uv.scripts]
start = "python app.py"
test = "pytest"
lint = "flake8"
```

Run scripts:

```bash
uv run start
```

```bash
uv run test
```

```bash
uv run lint
```