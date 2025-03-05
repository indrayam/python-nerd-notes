# uv

## uv install

- Install

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```
- Update

```bash
uv self update
uv tool upgrade --all
```

- Tools

```bash
{
uv tool install pycowsay
uv tool install huggingface-hub
uv tool install modal
uv tool install llm
uv tool install strip-tags
uv tool install symbex
uv tool install ttok
uv tool install yt-dlp
uv tool install datasette
uv tool install git+https://github.com/OpenInterpreter/open-interpreter.git@development
uv tool install shot-scraper
uv tool install files-to-prompt
uv tool install jc
uv tool install sqlite-utils
uv tool install playwright
}

{
uv tool install pycowsay --reinstall
uv tool install huggingface-hub --reinstall
uv tool install modal --reinstall
uv tool install llm --reinstall
uv tool install strip-tags --reinstall
uv tool install symbex --reinstall
uv tool install ttok --reinstall
uv tool install yt-dlp --reinstall
uv tool install datasette --reinstall
uv tool install git+https://github.com/OpenInterpreter/open-interpreter.git@development --reinstall
uv tool install shot-scraper --reinstall
uv tool install files-to-prompt --reinstall
uv tool install jc --reinstall
uv tool install sqlite-utils --reinstall
uv tool install playwright --reinstall
}
```


- Tools reinstall
```bash
uv tool install pycowsay --reinstall
```

## Useful commands

```bash
# version
uv version
uv -V

## run python tools in a temporary environment
uv tool run pycowsay Moo
uvx pycowsay Moo

## install python tools
uv tool install --help
uv tool dir
cd $HOME/.local/share/uv/tools
cd .local/bin

## list, install, uninstall
uv python list
uv python dir
uv python install 3.13
uv python install 3.14 --preview
uv python install --reinstall 3.13
uv python install --reinstall 3.14
uv python uninstall 3.13
uv python uninstall 3.14.0a3

## invoke any python version
uv run --python 3.14 python
uv run --python 3.13 --with torch python
uv run -p 3.12 --with torch --with numpy -- python

## play with standalone scripts
uv init --script hello.py --python 3.13
uv add --script hello.py 'torch' 'numpy'
# OR
touch hello.py
uv add --script hello.py --python 3.13 'torch' 'numpy'
# OR
touch hello.py
# create a requirements.txt file with 2 lines one for numpy and one for torch
uv add --script hello.py --python 3.13 --requirements requirements.txt

# uv ipython kernel setup
uv run ipython kernel install --user --env VIRTUAL_ENV $(pwd)/.venv --name=jupyter-apps-w-kernel

# Using uv pip to install packages without changing pyproject.toml
uv pip install tqdm

# Create a requirements.txt file based on pyproject.toml
uv pip compile pyproject.toml -o requirements.txt

```
