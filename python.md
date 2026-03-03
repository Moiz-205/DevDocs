### Python Documentation

A guide for **Python CLI commands**.

---

## Python Basics

- Check python version

```bash
python --version
```

- To run a script

```bash
py scripts.py
```

- To run a script in Interactive mode

```bash
py -i script.py
```

---

## Virtual Environment

- Create a virtual environment

```bash
py -m venv .venv
```

- Activate a virtual environment
1. Windows

```bash
.venv\Scripts\Activate.ps1
```

2. Linux

```bash
source .venv/bin/activate
```

- Deactivate a virtual environment

```bash
deactivate
```

- Remove the virtual environment directory

```bash
delete .venv
```

- Show virtual environment location

```bash
py -m venv --help
```

---

## Python Package Manager

#### *via PIP installer*

- Check pip version

```bash
pip --version
```

- Upgrade pip installer

```bash
py -m pip install --upgrade pip
```

- Install package

```bash
pip install package-name
```

    Flags

```bash
-q: Quite Mode
-U: Latest version
```

- List all packages

```bash
pip list
```

- Search specific package

```bash
pip search package-name
```

- Remove a package

```bash
pip uninstall package-name
```

- Create a requirements.txt file for the installed packages

```bash
pip freeze > requirements.txt
```

- Install packages from requirement.txt

```bash
pip install -r requirements.txt
```

---

#### *via UV package manager*

- Check UV version

```bash
uv --version
```

- Initialize project

```bash
uv init project-name
```

- Create virtual environment

```bash
uv venv .venv
```

- Activate virtual environment using UV

```bash
uv activate .venv
```

- Install package

```bash
uv add package-name
uv pip install package-name
```

- List installed packages

```bash
uv list
```

- Update a package

```bash
uv update package-name
```

- Deactivate virtual environment using UV

```bash
uv deactivate
```

- Remove virtual environment

```bash
uv remove .venv
```

- Rename virtual environment

```bash
uv rename old-name new-name
```

- Export virtual environment to YAML

```bash
uv export .venv > env.yaml
```

- Import virtual environment from YAML

```bash
uv import env.yaml
```

---

## Jupyter Notebooks

- Install Kernel Package

```bash
pip install ipykernel
```

- Install kernel on your machine

```bash
py -m ipykernel --user --name=.venv --display-name "Python (venv)"
```

- View installed kernels on your machine

```bash
jupyter kernelspec list
```

- Remove kernel from your machine

```bash
jupyter kernelspec remove .venv
jupyter kernelspec uninstall .venv
```

---

#### 
