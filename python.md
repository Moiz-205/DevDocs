### Python Documentation

A guide for **Python CLI commands**.

---

## Python Basics

- check python version

python --version

- To run a script

py scripts.py

- To run a script in Interactive mode

py -i script.py

---

## Virtual Environment

- Create a virtual environment

py -m venv .venv

- Activate a virtual environment
1. Windows

.venv\Scripts\Activate.ps1

2. Linux

source .venv/bin/activate

- Deactivate a virtual environment

deactivate

- Remove the virtual environment directory

delete .venv

---

## Python Package Manager

#### *via PIP installer*

- Check pip version

pip --version

- Upgrade pip installer

py -m pip install --upgrade pip

- Install package

pip install package-name

    Flags

-q: Quite Mode

-U: Latest version

List all packages

pip list

- Remove a package

pip uninstall package-name

---

## Jupyter Notebooks

- Install Kernel Package

pip install ipykernel

- Install kernel on your machine

py -m ipykernel --user --name=.venv --display-name "Python (venv)"

- View installed kernels on your machine

jupyter kernelspec list

- Remove kernel from your machine

jupyter kernelspecs remove .venv

jupyter kernelspecs uninstall .venv
