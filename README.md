# Multi year data visualization from Copernicus Marine toolbox

## Requirements
- a working package/file/environmnet manager like anaconda/miniconda or micromamba
- refer to the Archipelagos GIS Google Drive (contact Tim Grandjan for access request [here](t.grandjean@archipelago.gr)) or get instructions directly from the providers: [here](https://www.anaconda.com/download) for anaconda/miniconda, [here](https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html) for micromamba
- 
#### **1. activate copernicusmarine environment**
```bash
conda activate copernicusmarine
```
#### **2. install necessary libraries from requirements.yml**
```bash
conda env update --name copernicusmarine --file requirements.yml # find requirments.yml in this repository
```
#### **3. verify installation**
```bash
conda activate copernicusmarine
conda list  # Lists installed packages
```
