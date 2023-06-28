# Launch Pluto.jl from Jupyter

[![Latest PyPI version](https://img.shields.io/pypi/v/jupyter-pluto-proxy?logo=pypi)](https://pypi.python.org/pypi/jupyter-pluto-proxy)

Launch the awesome [Pluto.jl Notebook](https://plutojl.org/) from the
Jupyter Lab `Launcher` or the Jupyter Classic `New` dropdown. This
package was built using the [`jupyter-server-proxy` cookiecutter
template](https://github.com/illumidesk/cookiecutter-jupyter-server-proxy).

This is primarily for use with
[JupyterHub](https://github.com/jupyterhub/jupyterhub) in container
based environments.

## Launch

Take it for a spin with Binder:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/yuvipanda/jupyter-pluto-proxy/main?urlpath=pluto)

This should launch you straight into Pluto.

## Requirements

- [Python 3.6+](https://www.python.org/downloads/)
- [Docker](https://docs.docker.com/get-docker/)

## Installation

You can install `jupyter-pluto-proxy` from [PyPI](https://pypi.org/project/jupyter-pluto-proxy/).

```bash
pip install jupyter-pluto-proxy
```

You also need to have Julia and [Pluto.jl](https://github.com/fonsp/Pluto.jl)
installed.

## Launch

```bash
make build
```

The `make build` command creates your virtual environment with `virtualenv` and Python3, installs the required dependencies, and then launches your notebook with an arbritrary port with `repo2docker`.

## Development

1. Fork and clone this repo and install the package:

```bash
git clone https://github.com/<account>/jupyter-pluto-proxy
```

2. Create and activate a virtual environment:

```bash
virtualenv -p python3 venv
source venv/bin/activate
```

3. Install package:

```bash
cd jupyter-pluto-proxy
pip install -e .
```

## Credits

- [`jupyter-server-proxy`](https://github.com/jupyterhub/jupyter-server-proxy)
- [`Pluto.jl](https://github.com/fonsp/Pluto.jl)

## License

BSD 3-Clause
