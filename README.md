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
### Step 6: Loading the Shapefiles

Download the required shapefiles from the following GitHub repository:

[Download Shapefiles](https://github.com/lingling-liu/Hackathon_demo/tree/main/data)

After downloading, move the data from the `data/GBIF` folder into the following directory on your local machine:

```plaintext
C:/KIDS/data2024_0321/GBIF_Parallel_GIS_group/demo/
```
### Step 7: Run biodiversity_demo.ipynb

1. Copy the `biodiversity_demo.ipynb` notebook into your Jupyter Notebook.
2. Before running the notebook, change the paths to the shapefiles and data directories to match your local directory structure. Update the following code blocks in the notebook:

```python
# Load the shapefiles
gdf_shp = gpd.read_file("C:\\Path\\To\\Your\\Shapefile\\WB_countries_Admin0_10m.shp")
# Folder for GBIF
directory = "C:\\Path\\To\\Your\\Data\\GBIF_Parallel_GIS_group\\demo\\"

# Location for output pivot table
output_dir = "C:\\Path\\To\\Your\\Output\\Directory\\species\\demo\\"