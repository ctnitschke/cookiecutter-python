# My personal Python cookiecutter

## Structure

```
├── README.md        <-- The top-level README for users
├── .gitignore       <-- .gitignore with things I commonly don't want to check in in a Python project
├── pyproject.toml   <-- The project configuration file
└── src
    └── <package_name>   <-- The main package directory
        └── __init__.py  <-- A standard __init__.py file
```

## Baked-in tooling

### pytest with coverage

Testing.

### ruff

Linter.

### black

Code formatter.

### mypy

Type checker.

## Optional tooling

### PDM

I use [PDM](https://pdm-project.org/en/latest/) as package and dependency
manager because it suits my style. It works nicely with cookiecutter,
respects the standards well, is more versatile than `flit` and more
lightweight than `hatch`.
