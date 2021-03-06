# SpaceML Heliophysics Notebooks: Line-of-Sight Magnetogram (ML) Dataset

Heliophysics notebooks corresponding to the Magnetogram ML Dataset

## Notebooks:

* **01: SoHO/MDI & SDO/HMI Line-of-sight Magnetogram Dataset (2019)**
  * In this notebook, we demonstrate the process for interacting with a small sample of the HMI-MDI Magnetogram (ML) dataset. [publication in prep.]
  

*The following notebooks are currently under development*:

* **02: Super-resolution Magnetograms (2019)**
  * *Under development*, based on the FDL 2019 project to super-resolve SoHO/MDI and NSO/GONG Magnetograms to SDO/HMI resolution
* **03: NSO/GONG & SDO/HMI Line-of-sight Magnetogram Dataset (2019)**
  * *Under development*


## Interacting with each notebook:

Each notebook is contained within its own <project> folder:

```
.
└── notebooks
    └── ##_<project>_<year> # Each project has its own folder named sequentially, with the project name, and year of the project
        ├── README.md
        ├── <project>_colab.ipynb # A Jupyter notebook designed to be executed on Google Colab.
        ├── <project>.ipynb # The corresponding local development version of the colab notebook.
        ├── environment.yml # Conda environment file
        └── requirements.txt # Requirements file

```

For local development, the necessary environment can be created as follows (under the assumption that an anaconda installation exists).

```
cd notebooks/<project>
```

```
conda env create -f environment.yml
conda activate <environment>
```

```
# start the jupyter notebook app
jupyter notebook
```

## Contributions

Contributions are welcome as pull requests to the main branch, and should mirror the stucture of existing projects.

* A requirements file can be produced with `pip freeze > requirements.txt`, however, to minimize the nunmber of redundant packages in that list, first create a virtual environment, and `pip install` packages there (Anaconda is popular among scientists).

  ```
  conda create --name <name>
  conda activate <name>
  conda list #this should be empty
  ```

  

* Formatting with Black (https://black.readthedocs.io/en/stable/) is preferred; see https://github.com/drillan/jupyter-black for the Jupyter notebook integration:

  ```
  pip install black
  jupyter nbextension install https://github.com/drillan/jupyter-black/archive/master.zip --user
  jupyter nbextension enable jupyter-black-master/jupyter-black
  ```

  
