# Multi year data visualization with Copernicus Marine Toolbox

- this repository was mainly created for Archipelagos interns to maintain data harvesting from `Copernicus Ocean Products` for marine research purposes
- this is a 'from scratch guide' starting from anaconda installation and copernicus API setup to more sophisticated data querying and visualiazation

## Requirements
### Step 0:
- a working package/file/environment manager like anaconda/miniconda or micromamba with a Python > 3 installation:
  - refer to the Archipelagos GIS Google Drive (contact Tim Grandjan for access [here](mailto:t.grandjean@archipelago.gr)) or get instructions directly from the providers:
    - [here](https://www.anaconda.com/download) for anaconda/miniconda
    - [here](https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html) for micromamba

- an Interactive Development Environment (IDE) or a Notebook-based Interactive Computing Environment:
  - this repository was built using Jupyter lab (read more details [here](https://jupyter.org))
  - after sucessfull conda installation follow the next steps to get your instance
  - it is highly recommended to install Juypter lab in a seperate environment and link other environment Kernels to this one instance
 
    ```bash
    # Create and Activate a jupyter Environment
    conda create -n jupyter python=3.9 jupyterlab ipykernel -y
    conda activate jupyter
    ```
    
    ```bash
    # Install Juypter
    conda install -c conda-forge jupyterlab
    ```

### Step 1: Establish connection to Copernicus Server through the Copernicus Marine Toolbox

#### **1. Install the Toolbox from the conda-forge channel**
```bash
mamba create --name copernicusmarine conda-forge::copernicusmarine --yes
```

#### **2. Activate copernicusmarine environment**
```bash
conda activate copernicusmarine
```

#### **3. Verify installation**
```bash
conda list  # Lists installed packages
```

#### **4. Install a ipykernel**
```bash
# Inside the copernicusmarine environment, install the ipykernel package
conda install -c conda-forge ipykernel -y
```

#### **5. Register this environment as a Jupyter Kernel**
```bash
# This registers the copernicusmarine environment inside Jupyter
python -m ipykernel install --user --name copernicusmarine --display-name "CMT_Kernel"
```

### Step 2: Install necessary libraries 
```bash
conda env update --name copernicusmarine --file requirements.yml # find requirments.yml in this repository
```
## Usage

## Output

## Relevat References
