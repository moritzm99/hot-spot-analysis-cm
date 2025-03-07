# Multi year data visualization with Copernicus Marine Toolbox

## Requirements
### Step 0:
- a working package/file/environmnet manager like anaconda/miniconda or micromamba with a Python > 3 installation:
  - refer to the Archipelagos GIS Google Drive (contact Tim Grandjan for access [here](mailto:t.grandjean@archipelago.gr)) or get instructions directly from the providers:
    - [here](https://www.anaconda.com/download) for anaconda/miniconda
    - [here](https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html) for micromamba

- an Interactive Development Environment (IDE) or a Notebook-based Interactive Computing Environment:
  - this repository was built using Jupyter lab (read more details [here])
  - after sucessfull conda installation follow the next steps to get your instance
  - it is highly recommended to install Juypter lab in a seperate environment and link other environment Kernels to this one instance

### Step 1: Establish connection to Copernicus Server through the Copernicus Marine Toolbox

#### **1. Install the Toolbox from the conda-forge channel**
```bash
mamba create --name copernicusmarine conda-forge::copernicusmarine --yes
```



#### **1. Activate copernicusmarine environment**
```bash
conda activate copernicusmarine
```
#### **2. Install necessary libraries from requirements.yml**
```bash
conda env update --name copernicusmarine --file requirements.yml # find requirments.yml in this repository
```
#### **3. Verify installation**
```bash
conda activate copernicusmarine
conda list  # Lists installed packages
```
