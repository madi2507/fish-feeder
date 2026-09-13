# Fish Feeder AI

A hybrid AI system that combines machine learning and rule-based reasoning to make intelligent fish-feeding decisions.

## Overview

This project uses sensor information about a fish tank to determine whether fish are likely to be hungry and whether they should be fed.

The system combines:

- Machine Learning
- Rule-Based Reasoning
- Forward Chaining
- Uncertainty / Confidence-Based Reasoning

## How It Works

The system follows this pipeline:

**Sensor Data → Machine Learning → Fish Hunger Prediction → Rule-Based Reasoning → Final Feeding Decision**

### 1. Machine Learning

A Logistic Regression model is used to predict whether the fish are hungry.

The model uses features including:

- Water temperature
- Water clarity
- Hours since last feed
- Fish activity
- Ammonia level
- Nitrate level
- Light level

The data is preprocessed before training, including handling missing values and feature scaling.

The model achieved:

- Accuracy: 87.5%
- F1 Score: 0.878

### 2. Rule-Based Reasoning

The machine-learning prediction is then provided to a rule-based expert system.

The rule system uses sensor information and inferred facts to determine whether the fish should be fed.

Forward chaining is used to apply rules and derive new facts from the available information.

### 3. Final Decision

The final system combines the machine-learning prediction with rule-based reasoning to produce a feeding decision.

The system also represents uncertainty through confidence values, allowing the final decision to reflect the confidence of the reasoning process.

## Project Structure

- `Fish_feeder.ipynb` — main project implementation and experiments.
- `fish_feeder_report.docx` — detailed project report.

## Dataset

The original dataset was provided as part of a university competition and is no longer available to me, so it is not included in this repository.

The notebook contains saved outputs from the original project run.

## Technologies

- Python
- Jupyter Notebook
- Scikit-learn
- Logistic Regression
- Rule-Based Reasoning
- Forward Chaining
- Confidence-Based Reasoning
- Pandas
- Data Preprocessing

## Limitations

This project is an academic prototype. The rule-based system relies on predefined rules and may not cover every possible real-world fish-tank situation.

The machine-learning model was also developed using the available competition dataset and should not be treated as a production-ready autonomous feeding system.

## Author

**Madina**
