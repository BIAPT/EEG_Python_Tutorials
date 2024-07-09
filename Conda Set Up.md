# Coding Environment set up
 * Good idea to set up each project with dependencies/requirements 

To run Python scripts and work in Jupyter notebooks locally, download https://www.anaconda.com/
- Run the anaconda power shell
- It is good practice (for reproducibility) to instantiate a unique environment where all versions of packages are specified. 
- Follow the steps below for creating an environment, setting up jupyter and downaloading packages. 

# Create conda env
conda create -n myenv python=3.8

# Activate env(use deactivate to end)
conda activate myenv

# Install 
conda install -c conda-forge jupyterlab

# Requirements
mne, numpy, pandas... in a .txt file and install using "pip install XX"
