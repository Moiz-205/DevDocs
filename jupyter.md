### Jupyter Documentation

to setup venv for project
py -m venv <.venv>

to upgrade pip if outdated
py -m pip install --upgrade pip

to install packages (optional)
pip install <package-name>

to install ipykernel
pip install ipykernel

to setup kernel on your machine
py -m ipykernel --user --name <.venv> --display-name "Python (<Name>)"

to view kernels on your machine
jupyter kernelspec list

to remove kernel from your machine
jupyter kernelspec remove <.venv-name>
jupyter kernelspec uninstall <.venv-name>
