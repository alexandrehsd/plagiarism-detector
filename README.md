# Plagiarism Detector

## Getting Started

To run this project, first you'll need to install some packages in your operating system to make sure PyTorch runs smoothly. To do that: 

1. run `make install-dependencies`: this will install the system libraries necessary to run PyTorch.

Then, you need a virtual environment for python development. For that, you will need to install:

- [pyenv](https://github.com/pyenv/pyenv): Simple Python Version Management.
- [pyenv-virtualenv](https://github.com/pyenv/pyenv-virtualenv): A plugin that provides features to manage virtualenvs.

With those packages installed, you need to:

2. Run `make environment`: this will create a virtual environment with the name `plagiarism` and with python version 3.9.13. Done! You don't need to activate your environment, **pyenv** has automatically associated this project to your new `plagiarism` environment using a `.python-version` file.
3. Run `make requirements` to install all necessary packages.

## Running code

The project  takes place in the `notebooks/plagiarism_detector.ipynb` notebook. To run it, it is necessary to have at least 24 GB of RAM memory. So, if your machine does not satisfy this requirement, you can still run it by loading the precomputed artifacts that are inside the `artifacts` directory.

Loading precomputed artifacts is controlled by the variable `LOAD_PRECOMPUTED`, inside the notebook, which is set to `True` by default. To run the code from the ground up, just set `LOAD_PRECOMPUTED=False`.