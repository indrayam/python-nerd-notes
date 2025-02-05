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

# To get Matplotlib graphs to show up in the notebook
uv add sympy ipympl sympy_plot_backends
# To add interactivity, run this at the top of the notebook
# When I ran the command below, I got Javascript errors
# I just was not able to make ipympl work with the fancy 
# interactive plots that I wanted to use
%matplotlib widget

```