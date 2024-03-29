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

## AWS Setup
```
1. Used AWS ECR to store the copy of code on AWS Server.
2. Used IAM to create identity and stored secrete keys on github scerete store.
3. Used App Runner to deploy the app on AWS Server.
```

## MLflow

[Documentation](https://mlflow.org/docs/latest/index.html)


##### local cmd
- mlflow ui

### dagshub
[dagshub](https://dagshub.com/)

MLFLOW_TRACKING_URI=https://dagshub.com/RishavMishraRM/Dimond_Price_Prediction.mlflow \
MLFLOW_TRACKING_USERNAME=RishavMishraRM \
MLFLOW_TRACKING_PASSWORD=71e323f07937f6fb81cf857bcb75995b5ceab6f7 \
python script.py

Run this to export as env variables:

```bash

export MLFLOW_TRACKING_URI=https://dagshub.com/RishavMishraRM/Dimond_Price_Prediction.mlflow \
export MLFLOW_TRACKING_USERNAME=RishavMishraRM \
export MLFLOW_TRACKING_PASSWORD=71e323f07937f6fb81cf857bcb75995b5ceab6f7 \

```


### DVC cmd
- dvc init
- dvc repro -- to run the pipeline
- dvc dag




Folder Structure


```console
$ tree
.
│
├ .github
│    └── Workflow
│          ├── .gitkeep
│	       └──  YML Files
│
├── artifacts
│   ├── preprocessor.pkl
│   ├── model.pkl
│   ├── raw.csv
│   ├── test.csv
│   └── train.csv
│    
├── logs
│   └── log files
│    
├── Notebook
│   ├── Data
│   │    └── gemstone.csv(original data)
│   ├── research.ipynb
│   ├── Model_Training.ipynb
│   └── EDA.ipynb
│
├── SRC
│    └── DiamondPricePrediction
│              ├── Components
│              │     ├── __init__.py
│              │     ├── data_transformation.py
│              │     ├── data_ingestion.py
│              │     └── model_trainer.py
│              │  
│              ├── Pipelines
│              │     ├── __init__.py
│              │     ├── prediction_pipeline.py
│              │     └── training_pipeline.py
│              │  
│              │── Utils
│              │     ├── __init__.py
│              │     └── utils.py
│              │
│              ├── __init__.py
│              ├── exception.py
│              └── logger.py 
│  
│
├── templates
│   ├── form.html
│   ├── index.html
│   └── result.html
│
├── README.md
│
├── Dockerfile
│
├── .gitignore  
│
├── app.py
│
├── requirements.txt
│
├── LICENSE
│
├── setup.py
│
├── template.py
│
├── test.py
│
└── init_setup.sh
```
