# End-to-End Machine Learning Project


## Initializing Git with Github commands
```
git init
```
```
git add .
git add add.txt
```
```
git commit -m "This is my first commit"
```
```
git pull - to pull code from remote repo
```
```
conda create -n env python=3.8 -y
conda activate env

```

```
will run in gitbash/linux terminal
bash init_setup.sh
```

```
Pipeline -- Having all the components in one place
1. Data Ingestion
2. EDA
3. FE
4. Model Building
5. Model Evaluation

Pipeline - two types
1. Training Pipeline
2. Prediction or Testing Pipeline

```
```
Logger
1. exception logger - to log the exception
2. info logger - to log the info
```

```
Utils files - having all the standard functions
Setup.py file - to install local package
requirements.txt - to install all the packages
```


.gitkeep - to keep empty folders or files in GitHub


### To install local packages
```
python setup.py install
another way
pip install -r requirements.txt & (-e .) in the requirements.txt file
```

Folder Structure


```console
$ tree
.
│
├ .github
│    └── Workflow
│	   └──  YML Files
│
├── artifacts
│   ├── raw.csv
│   ├── test.csv
│   └── train.csv
│    
├── Notebook
│   ├── Data
│   ├── Model_Training.ipynb
│   └── EDA.ipynb
│
├── SRC
│    ├── DiamondPricePrediction
│    │         ├── Components
│    │         │     ├── __init__.py
│    │         │     ├── data_transformation.py
│    │         │     ├── data_ingestion.py
│    │         │     └── model_trainer.py
│    │         │  
│    │         ├── Components
│    │         │     ├── __init__.py
│    │         │     ├── prediction_pipeline.py
│    │         │     └── training_pipeline.py
│    │         │  
│    │         └── Utils
│    │               ├── __init__.py
│    │               └── utils.py
│    │
│    ├── __init__.py
│    ├── exception.py
│    └── logger.py   
├── README.md
├── .gitignore  
├── requirements.txt
├── LICENSE
├── setup.py
├── template.py
├── test.py
└── init_setup.sh
```
