# kidney-disease-classification
kidney-disease-classification

## Workflows
1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the dvc.yaml
10. app.py

# How to run?
 
### Steps:

Clone the repository

```bash
git clone https://github.com/aliakseibrown/kidney-disease-classification.git
```

### STEP 1 - Create a conda environment after opening the repository

```bash
conda create -n cnncls python=3.8 -y
```

```bash
conda activate cnncls
```

### STEP 2 - Install the requirements
```bash
pip install -r requirements.txt
```


##### cmd
- mlflow ui

### dagshub
[dagshub](https://dagshub.com/) 

MLFLOW_TRACKING_URI=https://dagshub.com/aliakseibrown/kidney-disease-classification.mlflow \
MLFLOW_TRACKING_USERNAME=aliakseibrown \
MLFLOW_TRACKING_PASSWORD=435491a5b08f4198a561a9bd44fbe9d89f59fa04 \
python script.py

Run this to export as env variables:

```bash
export MLFLOW_TRACKING_URI=https://dagshub.com/aliakseibrown/kidney-disease-classification.mlflow

export MLFLOW_TRACKING_USERNAME=aliakseibrown

export MLFLOW_TRACKING_PASSWORD=435491a5b08f4198a561a9bd44fbe9d89f59fa04

```

### DVC cmd

1. dc init
2. dvc repro
3. dvc dag