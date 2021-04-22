# End-to-End Machine Learning Project Template

_A logical, reasonably standardized, but flexible project structure for doing and sharing machine learning work._


### Requirements
-----------

Note: template tested on Python 3.8

Run:
``` bash
$ pip install requirements.txt
```

### Starting a New Project
------------
Run:

    cookiecutter https://github.com/mihail911/e2eml-cookiecutter


### Resulting directory structure
------------

The directory structure of your new project looks like this:

```
├── LICENSE
├── README.md          <- The top-level README for this project
│
├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
│                         generated with `pip freeze > requirements.txt`
│
├── assets             <- Stores any images, PDFs, or other static assets
│ 
├── data
│   ├── processed      <- The final, processed data sets for modeling
│   └── raw            <- The original, immutable data dump
│
├── deploy             <- Stores any files, configurations related to deploying your model (Dockerfile, etc.)
│ 
├── model_checkpoints  <- Trained and serialized models, model predictions, model summaries, config files
│
├── notebooks          <- Jupyter notebooks for doing exploratory data analysis, analyzing model outputs, etc.
│
├── scripts            <- Single-purpose scripts for functionality such as processing and cleaning data
│
├── tests              <- Tests for the various aspects of the project (data cleanliness, data processing, model training code, etc.)
│
├── {{cookiecutter.repo_name}}     <- Source code for use in this project
│   ├── __init__.py    <- Makes {{cookiecutter.repo_name}} a Python module
│   │
│   ├── model          <- Stores any relevant modeling code, interfaces, and definitions
│   │   └── __init__.py
│   │
│   ├── server         <- Stores deployment and inference server code
│   │   ├── __init__.py
│   │   └── main.py    <- Main module for running server
│   │
│   ├── utils          <- Stores various utilities used in project 
│   │   ├── __init__.py
│   │
│   ├── train.py       <- Script to run model training
│   └── eval.py        <- Script to run trained model evaluation 
```
