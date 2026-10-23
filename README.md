# Cyber-Attcak-prediction-Model

This project is made by student of the DSTI school. The objective is to develop a ML model to predict the type of attack. The project is composed of 3 main parts:

Exploratory Data Analysis.
Feature Engineering.
Model Development.
The repository includes:

A main notebook summarising our work.
A website to upload data and get prediction using our best model.
Scripts we made for each parts of the project.
Installation
You may clone the repository and then create a virtual environment and installing the required libraries.
Steps are:
1- Create virtual environnement using

python -m venv ./name_of_venv
2- Activate virtual environnement:

source ./name_of_venv/bin/activate
2- Install libraries:

pip install -r requirements.txt
If you plan to run a notebook that import the prince library run this command just after installing the libraries:

python scripts/patch_venv.py
Prince library is not up to date with pandas 3.X which creates a problem when using it. This quick patch solve the problem temporarily

Main Notebook
The main notebook (at the root of the repository) is a summary of all the work done by the team through the differents steps. It runs from top to bottom and features:

EDA part
Presentation of the dataset and the features.
A quick summary of the data describing data type, presence of missing values etc.
Analysis of the features
Short analysis of the features and how they are related to the attack types (distrubtion per attack type)
Website
We provice a website interface that can be used to upload cyber-attack dataset similar to the one used for the training of our model. Because the website was developed on another framework. A specific virtual environment must be used. To create it, use the following command:

python -m venv ./name_of_website_venv
source ./name_of_website_venv/bin/activate
pip install -r web_requirements.txt
After activating the web venv, to run the website, use the following command on the terminal

streamlit run Website/ui.py
Then open the following link.
