# Toxic Comment Classification

## Overview

This project focuses on classifying Wikipedia comments based on their toxicity. The types of toxicity include:

- toxic
- severe_toxic
- obscene
- threat
- insult
- identity_hate

The goal is to build a model that predicts the probability of each type of toxicity for a given comment.

Link for our models and results →

https://drive.google.com/drive/folders/1VjPzA_F612-AT6GVxXp2czKCWjX_0y6k?usp=sharing   (Download Trained Models From Here)

## Project Structure

This GitHub repository includes a folder named "Toxic_Comment_Classification_Api," which contains the FastAPI implementation for demonstrating the project.

File Structure for the same folder is as below

├── Classification_Api

│ ├── cleanText.py

│ ├── pred.py

│ ├── trainedModels.py

│ ├── main.py

│ ├── models

│ │ ├── model1.pkl

│ │ ├── model2.pkl

│ │ └── model3.pkl

| │ ...... Total 30-35 Models ----

├── notebook

│ ├── Toxic_Comment_Classification_ML.ipynb

| ├── result_on_toxic_comments.csv

| ├── test.csv

| ├── train.csv

└──README.md





### Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

### Installation

1. Clone the repository:

```bash
git clone https://github.com/KSN7630/Toxic-Comment-Classification.git
cd Toxic-Comment-Classification
``` 
2. Download Trained models from link :
```bash
https://drive.google.com/drive/folders/1VjPzA_F612-AT6GVxXp2czKCWjX_0y6k?usp=sharing   (Download Trained Models From Here)
```

Extract zip file into folder named "models"

3. Install the required packages:
```bash
pip install -r requirements.txt
```
4. Run the main.py file to start the FastAPI server, which will be accessible at http://127.0.0.1:8000/.


# Api Endpoints :

- POST /predict-comment: Predicts the toxicity levels of a given comment.

Example Request :
```bash
{
  "input_string": "Your Example Here"
}
```
Response :
```bash
{
    "Status": false,     #Shows overall Toxic or Not  --> true For Toxic
    "toxic": true/false,      
    "severe_toxic": true/false,
    "obscene": true/false,
    "threat": true/false,
    "insult": true/false,
    "identity_hate": true/false
}
```

## Screenshots

Here are some screenshots demonstrating the working API:

1) ![image](https://github.com/KSN7630/Toxic-Comment-Classification/assets/120741965/2af6b5ac-a217-4a01-b186-181b1b0a2713)

2) ![image](https://github.com/KSN7630/Toxic-Comment-Classification/assets/120741965/a2509c1b-07a9-4e95-a529-71e33489faae)




