# 🚨 Spam URL Detection System

## Project Overview
This project focuses on detecting spam URLs using Natural Language Processing (NLP) techniques and machine learning. The goal is to classify URLs as either spam or not spam based on their textual content. The model leverages the support vector machine (SVM) algorithm to build a classifier trained on a dataset of URLs labeled as spam or not.

---

## 📂 Project Structure

The project is organized as follows:

- spam_detection.ipynb - The main Python script.
- app.py - Python script.
- explore.py - A notebook to explore data, play around, visualize, clean, etc. 
- utils.py - This file contains utility code for operations like database connections.
- requirements.txt - This file contains the list of necessary python packages.
- models/ - This directory should contain your SQLAlchemy model classes.
- data/ - This directory contains the following subdirectories:
  - interin/ - For intermediate data that has been transformed.
  - processed/ - For the final data to be used for modeling.
  - raw/ - For raw data without any processing.

*Note*: This project structure is a general guideline and may not be strictly followed in every case. The actual structure might vary depending on the project needs, team preferences, or specific workflows.

---

## Dataset
The dataset consists of URLs labeled as spam (1) or not spam (0). It includes:
- **URL**: The URL string.
- **is_spam**: Label indicating whether the URL is spam or not.

The data contains noise and irrelevant information, which is preprocessed for better accuracy in the model.

---

## Objective
The primary goal of the project is to build a model that can accurately classify URLs as spam or not based on their text content.

---

## 📈 Key Features

### Data Preprocessing
- Cleaned and transformed the text of URLs by removing unwanted characters and irrelevant spaces.
- Lemmatized and removed stopwords to improve model performance.

### Feature Extraction
- Used TF-IDF vectorization to convert the text data into numerical features for the machine learning model.

### Model Building
- Built and evaluated a Support Vector Machine (SVM) model with a linear kernel to classify URLs.
- Optimized the SVM model with a grid search over multiple hyperparameters.

### Wordcloud Visualization
- Generated a word cloud to visualize the most frequent terms in the URLs.

---

## 🛠️ Technologies Used

| **Category**         | **Libraries/Tools**            |
|----------------------|--------------------------------|
| Programming Language | Python                         |
| Data Manipulation    | Pandas, NumPy                  |
| Text Preprocessing   | regex, NLTK                    |
| Visualization        | Matplotlib, WordCloud          |
| Machine Learning     | Scikit-learn                   |

---

## 📊 Performance Summary

| **Model**  | **Precision** | **Recall** | **F1-Score** | **Accuracy** |
|------------|---------------|------------|--------------|--------------|
| SVM        | 0.83          | 0.51       | 0.63         | 0.95         |

**Note**: The SVM model, after hyperparameter optimization, achieves a high accuracy but has room for improvement in recall for spam classification.

---

## 🚀 Getting Started

### Requirements
- **Python 3.8+**
- Install the required libraries:
  ```bash
  pip install pandas numpy matplotlib scikit-learn regex nltk wordcloud
How to Run:  
Clone the repository  
Follow the step-by-step analysis, preprocessing, and model evaluation process.

## 🌟 Highlights
Real-world Application: This system helps classify potentially harmful URLs, improving security and reducing spam.    
Reproducibility: Each step, from data preprocessing to model optimization, is well-documented for ease of use.    
Open Source Contribution: The code is available for further improvement and adaptation to other NLP classification tasks.    
## 📬 Contact
Author: Nathan Harroch  
LinkedIn: [linkedin.com/in/username ](https://www.linkedin.com/in/nathan-harroch-b11590196/)   
Email: nathan.harroch06@gmail.com    
