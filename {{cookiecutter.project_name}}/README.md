
# Project Name: {{cookiecutter.project_name}}

# The file structure of a standards powerpoint automation

└── {{cookiecutter.project_name}}
    ├── config
    │   └── 1_main.smk
    ├── {{cookiecutter.project_name}}.Rproj
    ├── data
    │   ├── calc
    │   ├── processed
    │   └── raw
    ├── docs
    ├── envs
    ├── output
    │   ├── ET
    │   └── powerpoint
    ├── README.md
    └── src
        ├── pp_auto
        └── r_precalc

# Map structure and use

## Folders:

data: This contains three subfolders called calc/processed/raw to illustrate the progress of the workflows data processing steps and also where you spect to find these diferent types of data.

docs: Here is where the metadata lives i.e the variable definition, labels, and statements mostly in form of a csv or excel document which can be easily changed at any time. Relevant subfolders should be cerated for further organization.

src: Usually the outomation project we have made som far have two kind of scipts, python and R, here they got a designated folder each.

output: The main workflow is based en a so called Enhance table(ET), which is a tidy long format results table to quality check and retrive data for powerpoint making. Here in the output folder the results are both the ET and powerpoint.

env: If we want to document the version of the packeges used in R and/or python we store a yml to later be able to recreate a conda environment, to run the exact workflow as it was mean to be.

config: Here we store the snakemake files to fully automate the workflow.

