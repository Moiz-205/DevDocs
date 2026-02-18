### Python Documentation

A guide for **Python CLI commands**.

---

## Python Basics

- check python version

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

List all packages

```bash
pip list
```

- Remove a package

```bash
pip uninstall package-name
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
jupyter kernelspecs remove .venv
jupyter kernelspecs uninstall .venv
```
