# {{cookiecutter.project_name}}

{{cookiecutter.project_description}}

# Contributing

# Development installation

{% if cookiecutter.environment_manager == "poetry" %}
This project uses `poetry` for environment management. If you haven't already, we recommend installing it with pipx:

```sh
pipx install poetry
```

After cloning the project from git, do

```sh
poetry sync
```

to create the environment and install all dependencies.
{% elif cookiecutter.environment_manager == "uv" %}
This project uses `uv` for environment management. If you haven't already, we recommend installing it with pipx:

```sh
pipx install uv
```

After cloning the project from git, do

```sh
uv sync
```

in order to install all dependencies.
{% elif cookiecutter.environment_manager == "venv/pip" %}
This project does its environment management "on foot". So, after cloning the project from git, it is recommended to
create a virtual environment using

```sh
python -m venv .venv
```

and activating it.

Then, install the project with

```sh
pip install --group dev -e .
```
{% endif %} 
