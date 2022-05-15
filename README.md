# SQAPlantilla with Cookiecutter

_A logical, reasonably standardized, but flexible project structure for doing and sharing machine learning work._

### Requirements to use the cookiecutter template:
-----------
 - Python 2.7 or 3.5
 - [Cookiecutter Python package](http://cookiecutter.readthedocs.org/en/latest/installation.html) >= 1.4.0: This can be installed with pip by or conda depending on how you manage your Python packages:

``` bash
$ pip install cookiecutter
```

or

``` bash
$ conda config --add channels conda-forge
$ conda install cookiecutter
```


### To start a new project, run:
------------

    cookiecutter https://github.com/DashaEscobar/SQAPlantilla

### The resulting directory structure
------------
The directory structure of your new project looks like this: 

    ├── LICENSE
    ├── README.md              <- The top-level README for developers using this project.
    ├── CITATION.cff           <- Way to cite this project.
    ├── CODE_OF_CONDUCT.md     <- Expected behavior rules from the community and the project owners.
    ├── CONTRIBUTING.md        <- Contribution rules for the project.
    ├── data
    │   └── raw                <- The original, immutable data dump.
    │
    ├── docs                   <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models                 <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks              <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                             the creator's initials (if many user development), 
    │                             and a short `_` delimited description, e.g.
    │                             `1.0-jqp-initial_data_exploration.ipynb`.
    │
    ├── references             <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports                <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures            <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt       <- The requirements file for reproducing the analysis environment, e.g.
    │                             generated with `pip freeze > requirements.txt`
    ├── test-requirements.txt  <- The requirements file for the test environment
    │
    ├── setup.py               <- makes project pip installable (pip install -e .) so {{cookiecutter.repo_name}} can be imported
    ├── src                    <- Source code for use in this project.
    │   ├── __init__.py        <- Makes {{cookiecutter.repo_name}} a Python module
    │   │
    │   ├── dataset            <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features           <- Scripts to turn raw data into features for modeling
    │   │   └── build_features.py
    │   │
    │   ├── models             <- Scripts to train models and make predictions
    │   │   └── deep_api.py    <- Main script for the integration with DEEP API
    │   │
    │   └── tests              <- Scripts to perfrom code testing
    │   │
    │   └── visualization      <- Scripts to create exploratory and results oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini                <- tox file with settings for running tox; see tox.testrun.org


--------

### Installing development requirements
------------

    pip install -r requirements.txt

### Running the tests
------------

    py.test tests