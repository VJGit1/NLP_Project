
#  Financial Complaint Categorization using NLP

### DATS 6312_11 - Final Group Project

This repository contains the code, analysis and final deliverables for our NLP project comparing classical machine learning techniques against modern transformer-based models for classifying consumer financial complaints.

##  Project Overview
The goal of this project is to automate the routing of financial complaints by classifying unstructured text narratives into specific product categories (e.g., "Mortgage", "Credit Card", "Debt Collection"). We utilize the Consumer Financial Protection Bureau (CFPB) database to train and evaluate models, focusing on handling class imbalance and PII redactions.

**Key Models Compared:**
* **Classical:** Multinomial Naive Bayes (TF-IDF features)
* **Transformer:** Fine-Tuned DistilBERT

##  Repository Structure

Here is an overview of the files and folders contained in this repository:

* **`Code/`**: Contains all Jupyter Notebooks for the project pipeline. This includes Exploratory Data Analysis (EDA), the Baseline Model, and the Transformer Model. Generated graphs and visualizations are also saved here.
* **`Final-Group-Project-Report/`**: Contains the detailed written report covering our methodology, results and conclusions.
* **`Final-Group-Presentation/`**: Contains the presentation slides used for the final project.
* **`NLP_Proposal.pdf`**: The original project proposal outlining our scope and objectives.
* **`.gitignore`**: Specifies intentionally untracked files to ignore (e.g., large datasets or system files).

##  Workflow Overview

The project is designed to be executed sequentially. For detailed technical instructions, please refer to the `README.md` inside the **Code** folder.

The general execution order is:

1.  **EDA**: Analyzes class distribution, n-grams, and word counts.
2.  **Baseline Model**: Trains and evaluates the Naive Bayes classifier.
3.  **Fine-Tuned DistilBERT**: Fine-tunes the transformer model and generates final comparisons.

##  Group Members
* Vaijayanti Deshmukh
* Amogh Ramagiri
* Lasya Raghavendra

---
*Course: DATS 6312 - Natural Language Processing for Data Science*
