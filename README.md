# Probabilistic Programming and Bayesian Computing with PyMC

### [SDSS 2024](https://ww2.amstat.org/meetings/sdss/2024/) Tutorial

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/fonnesbeck/pymc_sdss_2024/main) 

Bayesian statistical methods offer a powerful set of tools to tackle a wide variety of data science problems. In addition, the Bayesian approach generates results that are easy to interpret and automatically account for uncertainty in quantities that we wish to estimate or predict. Historically, computational challenges have been a barrier, particularly to new users, but there now exists a mature set of probabilistic programming tools that are both capable and easy to learn. We will use the newest release of PyMC (version 5), but the concepts and approaches that will be taught are portable to any probabilistic programming framework. This course is intended for practicing and aspiring data scientists and analysts looking to learn how to apply Bayesian statistics and probabilistic programming to their work. It will provide learners with a high-level understanding of Bayesian statistical methods and their potential for use in a variety of applications. They will also gain hands-on experience with applying these methods using PyMC, specifically including the specification, fitting and checking of models applied to a couple of real-world datasets. This is an introductory course, therefore no direct experience with PyMC or Bayesian statistics will be expected. However, to benefit maximally from the tutorial, learners should have some familiarity with basic statistical modeling (things like regression and estimation) and with core components of the scientific Python stack (e.g. NumPy, pandas and Jupyter). For those with no Python experience, some pre-conference tutorials will be posted to get new users up-and-running. This tutorial will be presented with Jupyter notebooks, allowing participants to run examples and exercises on their own computers. A GitHub repository will be set up 2 weeks prior to SDSS, with instructions on how to set up the Python environment to run the tutorial locally. As the goal of the tutorial is to get new users up and running with Bayesian methods, the content will be light on theory and focus on the implementation of models, though some statistical background will be provided for context and clarity. Since PyMC is a high-level statistical package, it is easy to gloss over important details of the underlying algorithms. Therefore, the tutorial will begin by solving a simple model using only NumPy and SciPy functions before diving into PyMC. As a capstone to the tutorial, learners will be introduced to "The Bayesian Workflow" to reiterate the important steps in the process, along with useful tips and tricks.

## Schedule

| Time     | Event                             |
|----------|-----------------------------------|
| 8:30-9:00 | Preliminaries                     |
| 9:00-10:45| Introduction to Bayesian Models   |
| 10:45-11:00| BREAK                             |
| 11:00-12:30| Building models in PyMC           |
| 12:30-13:30| LUNCH                             |
| 13:30-14:45| Fitting models with Markov chain Monte Carlo |
| 14:45-15:00| BREAK                             |
| 15:00-16:00| Hierarchical models               |
| 16:00-17:00| Model checking                    |
| 17:00-17:30| Closing Q&A                       |

## Setup

This tutorial assumes that you have some form of [Anaconda](https://www.anaconda.com/products/individual#download-section) Python (with Python version 3.11) setup and installed on your system. If you do not, please download and install this on your system before proceeding with the setup. We recommend using the [Miniforge](https://github.com/conda-forge/miniforge#download) distribution of Anaconda, which is a lightweight version of Anaconda that is easier to work with.

The next step is to clone or download the tutorial materials in this repository. If you are familiar with Git, run the clone command:

    git clone https://github.com/fonnesbeck/pymc_sdss_2024.git

otherwise you can [download a zip file](https://github.com/fonnesbeck/pymc_sdss_2024/archive/main.zip) of its contents, and unzip it on your computer.
***
The repository for this tutorial contains a file called `environment.yml` that includes a list of all the packages used for the tutorial. If you run:

    mamba env create

from the main tutorial directory (if you installed Anaconda instead of Miniforge, use `conda` instead of `mamba`), it will create the environment for you and install all of the packages listed. This environment can be enabled using:

    mamba activate bayes_course  

or 
    
    conda activate bayes_course

Then, you can start **JupyterLab** to access the materials:

    jupyter lab

The binder link above should also provide a working environment.

For those who like to work in VS Code, you can also run Jupyter notebooks from within VS Code. To do this, you will need to install the [Jupyter extension](https://marketplace.visualstudio.com/items?itemName=ms-toolsai.jupyter). Once this is installed, you can open the notebooks in the `notebooks` subdirectory and run them interactively.

#### If you are having issues with setting up your environment, please start a thread in the [Discussion forum](https://github.com/fonnesbeck/pymc_sdss_2024/discussions) for this repository. Time will also be allocated at the start of the tutorial to help with setup issues.