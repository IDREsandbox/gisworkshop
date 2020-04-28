# Introduction to GIS: Getting Started with Spatial Research

The following workshop is made available for the UCLA community. If you have a UCLA account, you can access the material for this workshop through IDRE's Jupyter notebooks by clicking <a href="https://jupyter.idre.ucla.edu/hub/user-redirect/git-pull?repo=https%3A%2F%2Fgithub.com%2FIDREsandbox%2Fgisworkshop&urlpath=lab%2Ftree%2Fgisworkshop%2F">here</a>. 

If you do not have a UCLA account, you can use the binder page below:

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/IDREsandbox/gisworkshop/master)

# Instructions to run locally

1. Clone this project into a local directory
1. Install Anaconda https://www.anaconda.com/products/individual
1. Launch Anaconda Navigator
1. Launch terminal, and run the following command:
    1. `pip install -r .\requirements.txt`
    
If you want to run in Jupyter Labs, follow these instructions:

Then run the following commands to install the required JupyterLab extensions (note that this will require node to be installed):
```
# Avoid "JavaScript heap out of memory" errors during extension installation
# (OS X/Linux)
export NODE_OPTIONS=--max-old-space-size=4096
# (Windows)
set NODE_OPTIONS=--max-old-space-size=4096

# Jupyter widgets extension
jupyter labextension install @jupyter-widgets/jupyterlab-manager@1.1 --no-build

# jupyterlab renderer support
jupyter labextension install jupyterlab-plotly@4.6.0 --no-build

# FigureWidget support
jupyter labextension install plotlywidget@4.6.0 --no-build

# Build extensions (must be done to activate extensions since --no-build is used above)
jupyter lab build

# Unset NODE_OPTIONS environment variable
# (OS X/Linux)
unset NODE_OPTIONS
# (Windows)
set NODE_OPTIONS=
```
