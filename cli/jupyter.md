# Jupyter

## Useful commands

```bash
# Jupyter subcommands
jupyter -h

# Jupyter subcommand help
jupyter kernelspec -h
jupyter kernelspec install -h

# List of kernels that jupyter knows about
jupyter kernelspec list
uv run jupyter kernelspec remove <name-of-kernel>

# OPTIONAL: If you're manually installing a custom or non-Python kernel, use jupyter kernelspec install. Otherwise, use the IPython kernel install command.
jupyter kernelspec install /path/to/my_kernel --user --name='myenv'

# List of paths
jupyter --paths

# Set JUPYTER_CONFIG_DIR to change the default configuration directory
jupyter --config-dir

# Set JUPYTER_DATA_DIR to change the default configuration directory
jupyter --data-dir
```