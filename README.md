# Template materials in Python

Example repository to create an environment with course materials in Python.

## Try it on Binder
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/sativa/template-python.git/master)


.. image:: https://mybinder.org/badge_logo.svg
 :target: https://mybinder.org/v2/gh/sativa/template-python.git/master


## Structure of the repo

This repository follows the [binder-examples/conda](https://github.com/binder-examples/conda) example very closely.

[`repo2docker`](https://repo2docker.readthedocs.io) is the underlying tool that is used to build an environment from a repository.

`repo2docker` can be configured with several types of files. In the case of this repo:

- `environment.yml`: specify the dependency that will be installed using `conda`
- `postBuild`: specify extra dependencies such as JupyterLab extensions

Once created, the environment can be reused without building it again.

For more information, see the [extensive rep2docker documentation](https://repo2docker.readthedocs.io).

## Materials

When building the environment, the materials (and any other file) will be copied to the Docker image.

In this example, there is already a test notebook available under `materials/example.ipynb`.
