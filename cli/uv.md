# uv

## Useful commands

```bash
uv version --help
uv -V
## run python tools in a temporary environment
uv tool run pycowsay Moo
uvx pycowsay Moo
## install python tools
uv tool install --help
uv tool dir
uv tool install pycowsay
cd $HOME/.local/share/uv/tools
uv tool install pycowsay
uv tool install llm
cd .local/bin
cd
which pycowsay
which llm
## install python versions
uv python dir
uv python find 3.13
uv python install 3.14 --preview
uv python install --reinstall 3.13
# invoke any python version
uv run --python 3.9 python
uv run --python 3.10 python
uv run --python 3.11 python
uv run --python 3.12 python
uv run --python 3.13 python
uv run --python 3.14 python
```
