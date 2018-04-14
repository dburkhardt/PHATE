PHATE  - Potential of Heat-diffusion for Affinity-based Transition Embedding
-------------------------------------------------------

PHATE is a tool for visualizing high dimensional single-cell data with natural progressions or trajectories. PHATE uses a novel conceptual framework for learning and visualizing the manifold inherent to biological systems in which smooth transitions mark the progressions of cells from one state to another. To see how PHATE can be applied to single-cell RNA-seq datasets from hematopoietic stem cells, human embryonic stem cells, and bone marrow samples, check out our preprint on BioRxiv.

[Kevin R. Moon, David van Dijk, Zheng Wang, et al. **PHATE: A Dimensionality Reduction Method for Visualizing Trajectory Structures in High-Dimensional Biological Data**. 2017. *BioRxiv*](http://biorxiv.org/content/early/2017/03/24/120378)


PHATE has been implemented in Python (2.7 and >=3.5), Matlab and R.


## Getting started

### Python installation and dependencies
1. The Python version of PHATE can be installed using:

        $ git clone --recursive git://github.com/SmitaKrishnaswamy/PHATE.git
        $ cd PHATE/Python
        $ python setup.py install --user

2. PHATE depends on a number of `python` packages available on pypi and these dependencies are listed in `setup.py`
All the dependencies will be automatically installed using the above commands

### MATLAB installation
1. The MATLAB version of PHATE can be accessed using:

        $ git clone --recursive git://github.com/SmitaKrishnaswamy/PHATE.git
        $ cd PHATE/Matlab

2. Add the PHATE/Matlab directory to your MATLAB path and run any of our `run_*` scripts to get a feel for PHATE.

### R version

#### Installation with `devtools`

The R version of PHATE can be installed directly from R with `devtools`:

        > if (!suppressWarnings(require(devtools))) install.packages("devtools")
        > devtools::install_github("KrishnaswamyLab/phater")

#### Installation from source

1. The R version of PHATE can be accessed [here](https://github.com/KrishnaswamyLab/phater), or by using:

        $ git clone --recursive git://github.com/SmitaKrishnaswamy/PHATE.git
        $ cd PHATE/phater
        $ R CMD INSTALL

2. If the `phater` folder is empty, you have may forgotten to use the `--recursive` option for `git clone`. You can rectify this by using:

        $ cd PHATE
        $ git submodule init
        $ git submodule update
        $ cd phater
        $ R CMD INSTALL

### Jupyter Notebook

A demo on PHATE usage and visualization for single cell RNA-seq data can be found in this notebook: [https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/PHATE_tree.ipynb](https://nbviewer.jupyter.org/github/KrishnaswamyLab/PHATE/blob/master/Python/tutorial/PHATE_tree.ipynb)
