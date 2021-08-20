# Efficient Online Estimation of Causal Effects by Deciding What to Observe

### Overview

This repository contains the implementation for the paper: <br>
__Efficient Online Estimation of Causal Effects by Deciding What to Observe__ [[PDF]](https://arxiv.org/pdf/) <br>
Shantanu Gupta, Zachary Lipton, David Childers

### Code and Datasets

The following Jupyter notebooks contain the code for running the experiments in our paper:

* `Linear_split_IV_graph.ipynb`: Code for the experiment for the instrumental variable (IV) graph (Figures 2a and 3a). 
* `Two_IVs_graph.ipynb`: Code for the experiment for the graph with two IVs (Figures 2b and 3b).
* `Confounder_mediator_graph.ipynb`: Code for experiment for the confounder-mediator graph (Figures 2c and 3c).
* `IHDP_data_graph.ipynb`: Code for the experiment with the Infant Health Development Program (IHDP) dataset (Figures 4a and 4b).
* `Vietnam_draft_earnings_data_graph.ipynb`: Code for the experiment with the Vietnam era draft and earnings dataset (Figure 4c).

The code depends on the Python libraries `numpy`, `scipy`, and `pandas`. In order to execute the iterations in parallel, we use the package [`ipyparallel`](https://ipyparallel.readthedocs.io/en/latest/).

The datasets and the code used for data preprocessing are located in the `data/` folder. The following files inside this folder contain the datasets used  
* `ihdp.RData`: The IHDP dataset taken from [Dorie, 2016](https://github.com/vdorie/npci/blob/master/examples/ihdp_sim/data/ihdp.RData).
* `ihdp_processed.csv`: The preprocessed IHDP dataset that we use in our experiments.
* `cpi_angrist1990.dta` and `cwhsc_new.dta`: The Vietnam era draft and earnings dataset taken from [Angrist, 2009](https://doi.org/10.7910/DVN/PLF0YL).
* `angrist_1951_cohort.csv`: The preprocessed Vietnam era draft and earnings dataset that we use in our experiments.

And the following files inside the `data/` folder contain the data preprocessing code:
* `IHDP_dataset_preprocessing.ipynb`: Code for preprocessing the IHDP data (generates `ihdp_processed.csv`).
* `Vietnam_draft_earnings_data_preprocessing.ipynb`: Code for preprocessing the Vietnam era draft and earnings dataset (generates `angrist_1951_cohort.csv`).

### Citation
If you find this code useful, please consider citing our work:
```bib
```
