# End to End Machine Learning Project

## initialize git first
```
git init
```
```
git add .
git add add.txt
```
```
git commit -m "this is my first commit"
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
Pipeline -- Haing all the components in one place
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
Utils files - having all the common functions
Setup.py file - to install local package
requirements.txt - to install all the packages
```


```
Github
||--> Workflow
||--> ---> YML files
||
||--> Notebook
||--> --> Research.ipynb
||
||--> src
||--> --> Dimond Price Prediction folder
||--> --> ---> Components
||--> --> ---> ---> Data Ingestion.py
||--> --> ---> ---> Preprocessing.py
||--> --> ---> ---> Model_training.py
||
||--> --> ---> Pipeline
||--> --> ---> ---> Training.py
||--> --> ---> ---> Prediction.py
||
||--> --> ---> exceptions.py
||--> --> ---> Logger.py
||--> --> ---> Utils.py
||
||--> requirements.txt
||--> setup.py
||

```

.gitkeep - to keep empty folder or files in github





