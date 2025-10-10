# Using mamba to create the IntroQG environment

## Starting steps

This briefly describes how to install a Python virtual environment for the Introduction to Quantitative Geology course.

1. Install micromamba following the instructions at https://mamba.readthedocs.io/en/latest/installation/micromamba-installation.html.
2. Clone the course Python environments from GitHub
    ```bash
    git clone https://github.com/introqg/python-environments.git
    ```
3. Change into the working directory with the cloned environment files
    ```bash
    cd python-environments
    ```

## Creating the environment for students

1. Create the python environment using micromamba
    ```bash
    micromamba env create -f introqg-student.yml
    ```
2. Activate the new environment and update JupyterLab
    ```bash
    micromamba activate introqg-student-2025
    sh postBuild
    ```
## Creating the environment for teachers

1. Create the python environment using micromamba
    ```bash
    micromamba env create -f introqg-teacher.yml
    ```
2. Activate the new environment and update JupyterLab
    ```bash
    micromamba activate introqg-teacher-2025
    sh postBuild
    ```
