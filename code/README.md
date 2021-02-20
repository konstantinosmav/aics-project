# Code
- The code folder contains two notebooks:
  - ai_project_preprocessing.ipynb mostly handles preprocessing of the dataset.
  - ai_project_model.ipynb creates datasets and dataloaders, contains the three different architectures of the models I built (that receive 2,3 and 4 features as input). One can simply load the csv files that are a result of ai_project_preprocessing. The models can either concatenate or sum the multimodal features – set concatenate to False to sum.
