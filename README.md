# Hackathon_demo
This is the demo for Biodiversity Hackathon.

# Installation

-   Install Mambaforge from https://github.com/conda-forge/miniforge#mambaforge
-   For convenience, during installation, I select yes for "Add Mambaforge to my PATH environment Variable"
-   (PC) Open the Miniforge Prompt (search for it in the start menu) or (Mac) just type "mamba init"
-   Create a new mamba environment with the following commands (here it is named env_kids):

`mamba create -n env_kids -c conda-forge`

-   Activate the environment

`mamba activate env_kids`

-   Install libraries using the mamba command:

`conda create -n gee python=3.11`
`conda activate env_kids`
`conda install ipykernel`
`python -m ipykernel install --user --name kids --display-name "Python (env_kids)"`
`conda install -n base mamba -c conda-forge`
`!pip install geopandas`
`conda install -c conda-forge geopandas`
`conda install -c conda-forge gdal`

-   Launch Jupyter notebook :

`jupyter notebook`
`%pip install ipywidgets`
`%pip install matplotlib`
