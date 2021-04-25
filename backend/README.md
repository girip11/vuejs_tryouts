# Fastapi Web application backend

## Project prerequisites

**Before opening the project workspace in VSCode, complete the installation of the prerequisites.**

### Pyenv installation

Pyenv is used for managing different versions of python. Pyenv installation instructions can be found [here](https://github.com/pyenv/pyenv#installation)

- Mac Os

  ```Bash
  brew update
  brew install pyenv
  ```

- Linux: Refer to the [pyenv-installer](https://github.com/pyenv/pyenv-installer) or [Pyenv github checkout](https://github.com/pyenv/pyenv#basic-github-checkout)

After installing pyenv, open a new terminal or source the `.bashrc` and execute the following commands.

```Bash
pyenv --version

# check if you can find version 3.8.6
pyenv install --list

pyenv install 3.8.6
```

```Bash
# execute the below command from within the backend folder
cd <path_to_fastapi_backend_folder>

# this sets the python version in the local directory to be 3.8.6
pyenv local 3.8.6

# verify the same using the following command
python --version
```

### Poetry installation

Poetry installation notes can be found [here](https://python-poetry.org/docs/)

```Bash
# execute the below command from within the backend folder
cd <path_to_fastapi_backend_folder>

# check if the python version is 3.8.6
python --version

python -m pip install poetry
```

### Setting up the virtual environment and Installing the dependencies

```Bash
# setup up the virtual environment and
# install all the project dependencies
poetry install --no-root

# help on commands provided by poetry
poetry --help

# options that can be given for a poetry command
poetry add --help

# Activates virtual environment
# This is very important.
poetry shell

# This can be used to run commands using the tools install in the
# virtual environment.
poetry run pip list
```

After installing the project dependencies, now visit **File -> open workspace** and then open the backend workspace.

## Running the project

- Open the terminal in the VSCode. Activate the virtual environment using `poetry shell` is not already activated.
- `uvicorn app.main:app --reload` starts the development server.

## Project structure

This project structure is inspired from the following

- [Fastapi postresql template](https://github.com/tiangolo/full-stack-fastapi-postgresql)
- [What are the best practices for structuring a FastAPI project?](https://stackoverflow.com/questions/64943693/what-are-the-best-practices-for-structuring-a-fastapi-project)

---

## References

- [Poetry documentation](https://python-poetry.org/docs/basic-usage/)
