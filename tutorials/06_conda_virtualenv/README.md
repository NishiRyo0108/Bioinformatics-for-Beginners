
# Conda & Virtual Environments

Learn to manage environments and dependencies with Conda.

## Learning Objectives
	•	Create, activate, export conda environments
	•	Install packages in isolated environments

## Simple Instructions
### Download  
- Method 1:   
[Download manually from github](https://github.com/conda-forge/miniforge/releases/tag/24.11.3-0)     
Linux：Miniforge3-Linux-x86_64.sh

- Method 2:
```bash
curl -L -O "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"

bash Miniforge3-$(uname)-$(uname -m).sh
```

Please read [miniforge3 guide](https://github.com/conda-forge/miniforge) for following instructions. 

### Initialization
```bash
~/miniforge3/bin/conda init
```
### Create virtual environment and install package

```bash
conda create -n bioinfo python=3.11
conda activate bioinfo
conda install pandas matplotlib
conda env export > environment.yml
```

### Update package

```bash
# update all packages in an environment
conda update -n [ENVIRONMENT] 
# or
conda update --all

# update single package in environment
conda install [PACKAGE]
```


🧪 Quiz     
	1.	How do you activate a conda environment?            
	2.	How do you export an environment file?      
	3.	Why use virtual environments?
