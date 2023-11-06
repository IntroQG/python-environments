# Using mamba to create the IntroQG environment

## Starting steps

This briefly describes how to install a Python virtual environment for the Introduction to Quantitative Geology course.

1. Install miniconda from https://docs.conda.io/en/latest/miniconda.html
2. Install mamba
    ```bash
    conda install mamba -n base -c conda-forge
    ```
3. Clone the course Python environments from GitHub
    ```bash
    git clone https://github.com/introqg/python-environments.git
    ```
4. Change into the working directory with the cloned environment files
    ```bash
    cd python-environments
    ```
## Creating the environment for students
1. Create the python environment using mamba
    ```bash
    mamba env create -f introqg-student.yml
    ```
2. Activate the new environment and update JupyterLab
    ```bash
    conda activate introqg-student
    sh postBuild
    ```
## Creating the environment for teachers
1. Create the python environment using mamba
    ```bash
    mamba env create -f introqg-teacher.yml
    ```
2. Activate the new environment and update JupyterLab
    ```bash
    conda activate introqg-teacher
    sh postBuild
    ```
