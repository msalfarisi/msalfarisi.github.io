---
title: "Jupyter notebook know-hows"
permalink: /tutorial/jupyter/
---

## Installation

First we neet to install mamba or conda. We can get started with the [miniforge](https://github.com/conda-forge/miniforge#mambaforge) distribution. In my case, I used Linux x86_64 (amd64) distribution compatible	**Mambaforge-Linux-x86_64**. The installation steps is as follows:

```
curl -L -O https://github.com/conda-forge/miniforge/releases/latest/download/Mambaforge-Linux-x86_64
bash Mambaforge-Linux-x86_64.sh
```

Then we need to restart the terminal.

Next, the installation of Jupyter follows. Here I used Jupyter notebook, which is used in web browsers. The [installation](https://jupyter.org/install) step using the previously installed mamba is as follows:

```
mamba install -c conda-forge notebook
```

To run the program, just type in the terminal:

```
jupyter notebook
```

Installing a package:

```
pip install -U scikit-learn scipy matplotlib
```

