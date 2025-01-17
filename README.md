# PowerFit3

## Acknowledgments
This project is forked from [Original Repo](https://github.com/original-author/original-repo).

## About PowerFit3

PowerFit3 is an updated version of the original PowerFit, designed to provide seamless compatibility with Python 3.9 while retaining all the core features and functionality that make PowerFit a powerful tool for cryo-EM density fitting.

PowerFit3 is a Python package and command-line program that automates the fitting of high-resolution atomic structures into cryo-EM densities. It employs a full-exhaustive 6-dimensional cross-correlation search to determine the optimal fit. Input requirements include an atomic structure in PDB format and a cryo-EM density file with its resolution. The output consists of positions and rotations of the atomic structure corresponding to high cross-correlation values.

Key features of PowerFit3 include:

+ Cross-Correlation Scoring: Uses the local cross-correlation function (CCF) as its primary scoring metric.
+ Enhanced Scoring Options: Includes Laplace pre-filtering and core-weighted versions to minimize overlapping densities from neighboring subunits.
+ Hardware Acceleration: Out-of-the-box support for multi-core CPUs and GPU acceleration via the OpenCL framework.
+ Multi-Platform Support: Compatible with Linux and macOS systems.

With the transition to Python 3.10, PowerFit3 ensures modern compatibility, improved maintainability, and future-proofing for users in computational structural biology. It remains open-source software, freely available to the community for scientific and educational purposes.


## Installation

You need to install conda first. [Miniforge](https://github.com/conda-forge/miniforge) is recommended.

(1) Create a conda environment by the following command:
```bash
    conda create -n powerfit3_env python=3.9
```
or
```bash
    mamba create -n powerfit3_env python=3.9
```

(2) After activating `powerfit3_env`. Install all necessary packages by

```bash
    pip install -r requirements.txt
```

(3) In powerfit3 root directory install powerfit3 by

```bash
    python setup.py install
```


If you want to run powerfit3 on gpu, you need to install gpyfft before step (3) via [gpyfft](https://github.com/geggo/gpyfft)


## Usage

The exactly same usage as the original work.


## Licensing

If this software was useful to your research, please cite us

If you use this package, please cite as the following:
```python
@article {Xie2024.09.16.613256,
	author = {Xie, Yuhao and Zhang, Chengwei and Li, Shimian and Du, Xinyu and Wang, Min and Hu, Yingtong and Liu, Sirui and Gao, Yi Qin},
	title = {Integrating various Experimental Information to Assist Protein Complex Structure Prediction by GRASP},
	elocation-id = {2024.09.16.613256},
	year = {2024},
	doi = {10.1101/2024.09.16.613256},
	publisher = {Cold Spring Harbor Laboratory},
	eprint = {https://www.biorxiv.org/content/early/2024/09/21/2024.09.16.613256.full.pdf},
	journal = {bioRxiv}

