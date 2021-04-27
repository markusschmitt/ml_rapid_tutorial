# Rapid tutorial for a few machine learning techniques

These are a few jupyter notebooks introducing basics of supervised learning, generative modelling, and reinforcement learning.
We discuss basic examples implemented in 
* Python with [JAX](https://github.com/google/jax) and [Flax](https://github.com/google/flax)
* Julia using the [Flux](https://fluxml.ai/Flux.jl/stable/) package.

## Set up Python environment

If you have [anaconda](https://www.anaconda.com/products/individual) installed, you can set up an environment with all required packages as follows:

1. Install Jupyter notebook and the `nb_conda_kernels` package in the base environment
```
    conda install -c conda-forge notebook
    conda install -c conda-forge nb_conda_kernels
```
2. Create a new environment
```
    conda create --name <insert_name_here> python=3.7 pip ipykernel ipywidgets tensorflow tensorflow-datasets matplotlib
```
3. Activate the new environment
```
    conda activate <insert_name_here>
```
4. Install JAX and Flax
```
    pip install jax jaxlib flax
```
5. Leave the new environment
```
    conda deactivate
```

Now you can open Jupyter notebook from the command line (with your `base` environment active) by entering
```
    jupyter notebook
```
In the notebook you should be able to choose a kernel named `Python [conda env:<insert_name_here>]`. When running this kernel, the libraries you just installed should be known.

Source: How to set up jupyter notebook to work with anaconda environments: https://towardsdatascience.com/how-to-set-up-anaconda-and-jupyter-notebook-the-right-way-de3b7623ea4a
