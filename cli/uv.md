# uv

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
uv tool install pycowsay
cd $HOME/.local/share/uv/tools
uv tool install pycowsay
uv tool install llm
cd .local/bin
cd
which pycowsay
which llm

## install and invoke python 
uv python dir
uv python find 3.13
uv python install 3.14 --preview
uv python install --reinstall 3.13
# invoke any python version
uv run --python 3.13 --with torch python
# invoke python with torch and numpy
uv run -p 3.12 --with torch --with numpy -- python

# Start a script for 3.13
uv init --script hello.py --python 3.13
uv add --script hello.py 'torch' 'numpy'
# OR
touch hello.py
uv add --script hello.py --python 3.13 'torch' 'numpy'
# OR
touch hello.py
# create a requirements.txt file with 2 lines one for numpy and one for torch
uv add --script hello.py --python 3.13 --requirements requirements.txt
```
