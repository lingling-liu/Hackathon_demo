# Biodiversity Hackathon Demo

This repository contains materials and instructions for participants of the Biodiversity Hackathon.

## Installation Instructions

### Step 1: Install Mambaforge

1. Download Mambaforge from [the official Conda-Forge page](https://github.com/conda-forge/miniforge#mambaforge).
2. During installation, choose "Yes" to add Mambaforge to your PATH environment variable.
3. For Windows, open the Miniforge Prompt from the start menu. For macOS, open a terminal and type `mamba init`.

### Step 2: Create and Activate a Mamba Environment

Create a new environment called `env_kids`:

```bash
conda create -n env_kids python=3.11
mamba activate env_kids
```
### Step 3: Step 3: Install Necessary Libraries
```bash
conda install -n base mamba -c conda-forge
mamba install geopandas -c conda-forge
conda install ipykernel
python -m ipykernel install --user --name kids --display-name "Python (env_kids)"
conda install -c conda-forge geopandas
conda install -c conda-forge gdal
```
### Step 4: Launch Jupyter Notebook
```bash
jupyter notebook
```
###  Step 5: Install Additional Python Packages
```bash
%pip install ipywidgets
%pip install matplotlib
```

## Loading the Shapefiles
Download the required shapefiles from the following GitHub repository:
Download Shapefiles






