
# Setup env

To manage package dependencies, conda was used. Steps:
* install conda (if you haven't yet)
* create a virtual env for this project

## install conda (if you haven't yet)
Download and install it: https://www.continuum.io/downloads

## Creating a virtual env

To create a project with all dependencies, you can run the following command in 
the terminal, after you have navigated to the root of this project.
```
conda create -n brfss-r-env -c r --file conda-requirements-r.txt
```
This will create a new virtual env based called "brfss-r-env", and with packages installed specified in file "conda-requirements-r.txt".

Whenever you want to run the scripts in R you created in the terminal, you just need to activate the venv, like the following.

To activate the env:
```
source activate brfss-r-env
```

To deactivate the conda env:
```
source deactivate
```

## Using jupyter notebook (optional)

After having setup your local environment, you can optionally run this code with a jupyter notebook. Run the following command in the root of this project (after having activated the conda env):
```
jupyter notebook
```




