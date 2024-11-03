# Antimicrobial Drug Resistance Prediction

This project utilizes machine learning models to predict antimicrobial resistance (AMR) based on genomic and DNA sequence data. The goal is to accurately classify microorganisms that may contain AMR markers, using multiple models to identify patterns in the data.

## Table of Contents
- [Overview](#overview)
- [Installation](#installation)
- [Usage](#usage)
- [Results](#results)
- [Model Performance](#model-performance)

## Overview

Antimicrobial resistance is one of the biggest threats to global health today. This project aims to contribute by building machine learning models that can predict AMR from genomic data.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/IamFaisal11/antimicrobial_drug_resistance.git
   
2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   
## Usage
   To train the models and evaluate performance, run the appropriate cells in this notebook
   
## Results
![Confusion Matrix](Results/output.png)

## Model Performance
The table below shows the best performing models along with their respective scores and optimal hyperparameters:

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Model Performance Table</title>
    <style>
        table {
            width: 50%;
            border-collapse: collapse;
            margin: 20px auto;
        }
        th, td {
            border: 1px solid #ddd;
            padding: 8px;
            text-align: left;
        }
        th {
            background-color: #f2f2f2;
        }
    </style>
</head>
<body>

    <h2 style="text-align: center;">Model Performance Table</h2>
    <table>
        <thead>
            <tr>
                <th>Model</th>
                <th>Best Score</th>
                <th>Best Parameters</th>
            </tr>
        </thead>
        <tbody>
            <tr>
                <td>SVM</td>
                <td>0.997887</td>
                <td>{'C': 1, 'kernel': 'linear'}</td>
            </tr>
            <tr>
                <td>Random Forest</td>
                <td>0.999736</td>
                <td>{'n_estimators': 1}</td>
            </tr>
            <tr>
                <td>Logistic Regression</td>
                <td>0.975431</td>
                <td>{'C': 10}</td>
            </tr>
        </tbody>
    </table>

</body>
</html>

These results indicate that the Random Forest model achieved the highest accuracy, followed closely by SVM. Adjusting the parameters for each model helped optimize performance, demonstrating that even small tweaks can significantly affect model accuracy for AMR prediction.

