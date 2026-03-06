## Python 3.13.12 configuration for Fish shell via UV

Install UV package manager first

```fish
curl -LsSf https://astral.sh/uv/install.sh | sh
```

Install Python 3.13.12 via UV

```fish
uv python install 3.13
```

Make Python 3.13.12 global

```fish
uv python pin --global 3.13
```

Check the Python currently being set as global

```fish
which python
python --version
```

Edit Fish .config file and add following

```nano
source $HOME/.local/bin/env.fish
set -gx PATH $HOME/.local/share/uv/python/cpython-3.13-linux-x86_64-gnu/bin $PATH
```

Restart Terminal and Run the following

```fish
which python
python --version
```

Python 3.13.12 all set up!
