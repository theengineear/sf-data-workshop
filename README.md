# Programmatic Data Visualization with Plotly in Python

## Requirements

For simplicity, I'll be running all of these notebooks in Python 2.7. However, all the packages support Python 3 just as well.

This set of notebooks requires the following:

* Please visit https://plot.ly and create an account (free)
* Please install the following packages `numpy`, `pandas`, and `plotly`
* Please follow the instructions at https://plot.ly/python/getting-started/

### Virtual environments and Jupyter notebooks

If you are using a virtual environment (a good choice), you'll need to do a little extra footwork. After you've created a virtual environment (I'll assume you know how to do this if you're choosing this solution), you need to create a new Python kernel for your notebook server.

Here's the documentation on it: https://ipython.readthedocs.io/en/stable/install/kernel_install.html#kernels-for-different-environments

It boils down to `pip`-installing `ipykernel` and running the following command (after you've activated your virtual environment):

`python -m ipykernel install --user --name <myenv> --display-name "Python (<myenv>)"`

Where `<myenv>` should be a string that you will use to organize your kernels. For example, I did something like the following to prepare for this workshop:

```bash
$ virtualenv sf-data
$ cd sf-data
$ source bin/activate
$ python -m ipykernel install --user --name sf-data --display-name "Python (sf-data)"
```

When I create a new notebook, I can now see `Python (sf-data)` as one of the kernel choices.

## Helpful links

Plotly has a *ton* of documentation to pull from you can access it all at https://plot.ly/python/. Here's a short list of topics we're going to gover here.

* [Getting Started](https://plot.ly/python/getting-started/)
* [Offline Plotting](https://plot.ly/python/offline/)
* [Figure Reference](https://plot.ly/python/reference/)
* [Cheat Sheet](https://images.plot.ly/plotly-documentation/images/python_cheat_sheet.pdf)

## Overview

In this tutorial, we're going to go from a simple "Hello World" example to creating complex, beautiful plots in Plotly with Python. The goal is not to give a talk, but rather to work through examples with everyone. Specifically, we'll cover:

* Getting Started (basic setup for using the `plotly` module.
* Plotting Commands
* Offline Plotting
* The `figure_factory` module
* Validation of figures and graph objects
* Animations
* A Real-World Example of Data Exploration
