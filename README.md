# notebooks

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sequgen/notebooks/HEAD?urlpath=lab)

Jupyter notebook demo of [sequgen](https://github.com/sequgen/sequgen) functionality.

## Prerequisites

For running locally on Ubuntu:

```shell
sudo apt install git
```

## Running the notebooks locally

First clone this repository.

```shell
git clone https://github.com/sequgen/notebooks.git .
```

Install the dependencies with

```shell
# Create a virtualenv, e.g. with
python3 -m venv env

# activate virtualenv
source env/bin/activate

# make sure to have a recent version of pip
pip install --upgrade pip wheel

# (from the repository root directory)
# install sequgen + jupyter
pip install --requirement requirements.txt

# add the new local environment to jupyter
ipython kernel install --name sequgen-demo --user
```

Start the notebook server:

```shell
jupyter lab
```

It will open a web browser with the Jupyter Lab environment, in file-browser on left side bar open the notebook (\*.ipynb files) of interest. Select the kernel `sequgen-demo` to run the notebook.
