# HTTP Request Attack Classification Using Machine Learning

A cybersecurity machine-learning project for detecting and classifying HTTP requests into normal traffic and common web-attack categories.

## Project Overview

This project develops and evaluates a Random Forest classifier for multiclass HTTP attack detection.

The workflow includes:

- Data preparation and cleaning
- Feature engineering and selection
- Class balancing using SMOTE
- Random Forest classification
- Hyperparameter tuning with GridSearchCV
- Model evaluation
- Prediction confidence analysis
- Adversarial robustness testing

## Attack Categories

The model classifies HTTP requests into six categories:

- Normal
- SQL Injection
- XSS
- Path Traversal
- Command Injection
- Other Anomalous

## Key Results

The fine-tuned Random Forest model achieved:

| Metric | Result |
|---|---:|
| Accuracy | 82.15% |
| Weighted F1 Score | 82.16% |

The model was compared against a baseline Random Forest model and improved through feature selection and hyperparameter tuning.

## Machine Learning Approach

### Features

The model uses engineered numerical features derived from HTTP requests, including:

- Request length
- Number of parameters
- SQL keyword indicators
- XSS pattern indicators
- Path traversal indicators
- Command injection indicators
- Special character count
- Encoded character count
- Path depth
- Digit count
- Uppercase character count

### Model

**Random Forest Classifier**

Hyperparameter tuning was performed using **GridSearchCV**.

### Class Balancing

**SMOTE (Synthetic Minority Over-sampling Technique)** was used to address class imbalance in the training data.

## Adversarial Evaluation

The project also evaluates model behavior under adversarial perturbations using the **Adversarial Robustness Toolbox (ART)**.

The model was tested at multiple perturbation levels to examine how classification performance changed under adversarial conditions.

An adversarial-training experiment was also performed and compared with the original fine-tuned model.

## Technologies

- Python
- Scikit-learn
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Imbalanced-learn
- Adversarial Robustness Toolbox (ART)
- Google Colab
- Jupyter Notebook

## Skills Demonstrated

- Cybersecurity machine learning
- HTTP attack detection
- Feature engineering
- Data preprocessing
- Class imbalance handling
- Model tuning and evaluation
- Random Forest classification
- Adversarial ML evaluation
- Python data analysis

## Notebook

The complete project workflow is available in:

`http_attack_classification_portfolio.ipynb`

The notebook can also be opened directly in Google Colab using the **Open in Colab** button.

---

**Author:** Alicia Lancaster  
**Cybersecurity Student | Fanshawe College**
