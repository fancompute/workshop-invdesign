# Optical Inverse Design with Automatic Differentiation

This repository contains the code and notebooks for the workshop on the inverse design of optical devices with automatic differentiation.

## Getting started

To get started using these course materials, you can transfer them to your local computing environment either by downloading them or git cloning this repository. To download a zip archive of these materials, simply click the green "Clone or download" button on the top right corner of the GitHub repository page and then selecting "Download ZIP" from the drop down menu.

If you have `git` installed, you can enter the following command in a terminal to clone the repository for the materials to your computer:

    git clone https://github.com/fancompute/workshop-invdesign.git

You will also need a python environment with the necessary packages installed in your local environment. There are several ways to setup a python environment, but we recommend using Anaconda. You can download the Anaconda installer for your operating system from: <https://www.anaconda.com/distribution/>. 

**Note:** you will want to install a 3.X version of Python (e.g. 3.6 or 3.7). By default, the Anaconda distribution includes many of the python packages that we require for this workshop. However, there are a few additional package we will need to manually install, as described in the next sections of this guide.

## Installing HIPS autograd

[HIPS autograd](https://github.com/HIPS/autograd) is an automatic differentiation framework with a Numpy-like API. We rely autograd for flexible gradient computation in our inverse design studies. To install autograd, execute the following command in your conda environment:

    pip install autograd

## Installing pymkl

pymkl provides an interface to the [PARDISO](https://www.pardiso-project.org/) sparse solver which we use to accelerate our simulations. To install pymkl, execute the following command in your conda environment:

    pip install pymkl

## Installing ceviche

Ceviche is our research group's finite difference frequency domain (FDFD) and time domain (FDTD) package. The source code is freely available on GitHub at <https://github.com/twhughes/ceviche>. You can install ceviche by git cloning the repository into your local computing environment and adding its location to your `PYTHONPATH` environment variable. However, we recommend installing ceviche via pip, by executing the following command:

    pip install ceviche

## Using the materials

The materials in this repository are organized into [Jupyter](https://jupyter.org/) notebooks. You can interact with them through the `jupyter lab` interface, which is a web-based user interface that runs from your local computing environment.
