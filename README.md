# notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sequgen/notebooks/main?filepath=demo.ipynb)

Jupyter notebook demo of [sequgen](https://github.com/sequgen/sequgen) functionality.

## Prerequisites

For running locally on Ubuntu:

```shell
sudo apt install jupyter-core
sudo apt install jupyter-notebook
sudo apt install git
```

## Running the notebooks locally

```shell
# Create a virtualenv, e.g. with
python3 -m venv venv-sequgen-demo

# activate virtualenv
source venv-sequgen-demo/bin/activate

# make sure to have a recent version of pip
pip install --upgrade pip wheel

# (from the project root directory)
# install sequgen
pip install --no-cache-dir git+https://github.com/sequgen/sequgen@ef89edb8f0fed866f3455db3852d5474f0b8a009

# install ipykernel
pip install ipykernel
python3 -m ipykernel install --user --name=sequgen-demo
```

Check to see if it all worked by listing the packages that are present in the environment:

```shell
pip list
```

This should yield a table of packages alongside where they were installed from. If everything looks OK, start the
notebook server:

```shell
jupyter notebook
```

And open a browser to http://localhost:8888 to interact with the notebook.
