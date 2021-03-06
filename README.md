[![Documentation Status](https://readthedocs.org/projects/dppy/badge/?version=latest)](https://dppy.readthedocs.io/en/latest/?badge=latest)
[![Build Status](https://travis-ci.com/guilgautier/DPPy.svg?branch=master)](https://travis-ci.com/guilgautier/DPPy)

# DPPy: Sampling Determinantal Point Processes with Python

> Anything that can go wrong, will go wrong. − [Murphy's Law](http://phdcomics.com/comics/archive.php?comicid=1867)

## Introduction

Determinantal point processes (DPPs) are specific probability distributions over clouds of points that have been popular as models or computational tools across physics, probability, statistics, and more recently of booming interest in machine learning. 
Sampling from DPPs is a nontrivial matter, and many approaches have been proposed. 
DPPy is a Python library that puts together all exact and approximate sampling algorithms for DPPs.

## Requirements

DPPy works with [Python 3.4+](http://docs.python.org/3/)

### Dependencies
 - [NumPy](http://www.numpy.org)
 - [SciPy](http://www.scipy.org/)
 - [Matplotlib](http://matplotlib.org/)
 - [Networkx](http://networkx.github.io/)

The `zono_sampling` mcmc sampler for finite DPPs requires CVXOPT which itself requires GCC
 - [CVXOPT](http://cvxopt.org)
 - [GCC](http://gcc.gnu.org)
    - On MAC it comes with [Xcode](https://developer.apple.com/xcode/)
    - On UNIX, use your package manager (`apt`, `yum` etc)
        ```bash
        sudo apt install -qq gcc g++
        ```

## Download
### Install from sources

Clone this repository

```bash
git clone https://github.com/guilgautier/DPPy.git
cd DPPy
```

And execute `setup.py`

```bash
pip install .
```

### How to cite this work?

We wrote a companion paper to [DPPy](https://github.com/guilgautier/DPPy) for latter submission to the [MLOSS](http://www.jmlr.org/mloss/) track of JMLR.

The companion paper is available on:
    - [arXiv](http://arxiv.org/abs/1809.07258)
    - [GitHub](https://github.com/guilgautier/DPPy_paper), see the [`arxiv`](https://github.com/guilgautier/DPPy_paper/tree/arxiv) branch

If you use this package, please consider citing it with this piece of BibTeX
```bibtex
@article{GaBaVa18,,
    archivePrefix = {arXiv},
    arxivId = {1809.07258},
    author = {Gautier, Guillaume and Bardenet, R{\'{e}}mi and Valko, Michal},
    eprint = {1809.07258},
    journal = {ArXiv e-prints},
    title = {{DPPy: Sampling Determinantal Point Processes with Python}},
    keywords = {Computer Science - Machine Learning, Computer Science - Mathematical Software, Statistics - Machine Learning},
    url = {http://arxiv.org/abs/1809.07258},
    year = {2018},
    note = {Code at http://github.com/guilgautier/DPPy/ Documentation at http://dppy.readthedocs.io/}
}
```

## Reproducibility

We would like to thank [Guillermo Polito](https://guillep.github.io/) for leading our reproducible research [workgroup](https://github.com/CRIStAL-PADR/reproducible-research-SE-notes), this project owes him a lot.

Take a look at the corresponding [booklet](https://github.com/CRIStAL-PADR/reproducible-research-SE-notes) to learn more on how to make your research reproducible!