[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/pjvBqEwI)
# 1. Assignment: News Classification

## Prerequisites

1. Create a venv by running `python -m venv venv`
1. Install the required packages. You can do this by running `pip install -r requirements.txt` in the `venv` directory.
1. Make sure you have Jupyter Notebook installed in your virtual environment. If not, run `pip install jupyter`.

## Environment Setup

1. Navigate to the directory where you created the virtual environment.
1. Activate the virtual environment:
	- On WSL/Linux: `source venv/bin/activate`
	- On Windows with PowerShell:
	```powershell
	.\venv\Scripts\Activate.ps1
	```
	- On Windows with Command Prompt:
	```cmd
	.\venv\Scripts\activate.bat
	```
1. Activate (`source venv/bin/activate` on WSL/Linux) the virutal environment.
	On Windows with activate the environment with PowerShell:
	```powershell
	.\venv\Scripts\Activate.ps1
	```
	or on Windows with Command Prompt:
	```cmd
	.\venv\Scripts\activate.bat
	```
1. install all requirements for the exercises (`pip install -r requirements.txt`).

Every assignment should be completed in a Jupyter notebook. Start the jupyter server
with the following command:
```bash
jupyter notebook
```

## Tasks

In the data directory you'll find files of the following dataset:
https://tblock.github.io/10kGNAD/^

The dataset contains german news articles.

Start the existing notebook, and add code to complete the following tasks:
1. Load the data, and remove rows with empty values (if exists) and duplicates
1. Remove stopwords and convert the text to lowercase (this might help: https://www.nltk.org/howto/corpus.html#word-lists-and-lexicons)
1. Encode the labels
1. Create a train/test split (80/20%) with stratified labels
1. train a logistic regression classifier with tf/idf feature vectors
1. train 2 other scikit learn models (e.g. RandomForestClassifier and LinearSVC)
1. Compare results based on accuracy and macro/micro f1-score (https://scikit-learn.org/stable/modules/generated/sklearn.metrics.f1_score.html)
