# Conda environment set up instructions for capstone project

## Install Miniconda
1. Log into server. Open a Terminal.
2. In terminal, run `wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh`
3. After download complete, run `bash Miniconda3-latest-Linux-x86_64.sh`. Accept all defaults.
4. Add `conda` to your PATH variable by running `nano ~/.bashrc`, and adding this line to the bottom of the file: `export PATH="~/miniconda3/bin:$PATH"`
5. Run `source ~/.bashrc` to update your PATH variable. Run `conda --version` and make sure that conda is properly installed; it should return the version number.

## Create the `capstone` conda environment
1. Download/copy+paste the `environment.yml` file in this repository to your project folder.
2. In the terminal, change to the project folder directory containing the `environment.yml` file.
3. Run `conda env create -f environment.yml` to re-create the `capstone` conda environment. It should install the libraries as specified in the `environment.yml` file.
4. After it completes installing the libraries, run `conda activate capstone` to activate the conda environment.
5. Run `jupyter lab` to start a Jupyter Lab instance. A Firefox window should pop up with a running JupyterLab session. You can work on your notebooks from here.
