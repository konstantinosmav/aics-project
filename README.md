# Project for the AICS course (MLT LT2318)

This is a repository contains a set file structure for submitting your project in this course.

See `library/github-instructions.md` for a description how to use this repository.

Use this file to keep general notes about your project, including your individual project plan. We will also use it for comments.


## Notes
-  The code folder contains two notebooks: 
  - ai_project_preprocessing.ipynb mostly handles preprocessing of the dataset. 
  - ai_project_model.ipynb creates datasets and dataloaders, contains the three different architectures of the models I built (that receive 2,3 and 4 features as input). One can simply load the csv files that are a result of ai_project_preprocessing. The models can either concatenate or sum the multimodal features – set concatenate to False to sum.
-  My actual notes are in the notes folder, where I keep a diary of my work progress.
-  The data folder contains links and instructions to retrieve the data needed to run the models.
-  The paper folder contains my presentation slides and my project report.
