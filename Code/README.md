#  NLP Project Code

This folder contains the code, datasets and generated visual assets required to execute the "Comparative Analysis of Classical and Transformer-Based Models" project.

##  Execution Order

To reproduce the results presented in the report, please execute the notebooks in the following order:

### 1. `EDA.ipynb` (Exploratory Data Analysis)
* **Purpose:** Loads the raw `complaints.csv` data and performs initial inspection.
* **Key Actions:**
    * Identifies class imbalances.
    * Discovers the "Credit Reporting" label duplication issue.
    * Identifies PII redaction patterns (e.g., `xxxx`).
    * Analyzes word count distributions to determine token length for the Transformer model.
* **Outputs:** `class_imbalance_plot.png`, `complaints_over_time.png`, `word_count_distribution.png`.

### 2. `Baseline Model.ipynb`
* **Purpose:** Establishes a performance benchmark using a Classical Machine Learning approach.
* **Key Actions:**
    * Implements text preprocessing (removing `xxxx`).
    * Vectorizes text using **TF-IDF**.
    * Trains a **Multinomial Naive Bayes** classifier.
    * Calculates the Macro F1-Score.
* **Outputs:** `baseline_confusion_matrix.png`.

### 3. `Fine_tuned_DistilBERT.ipynb`
* **Purpose:** Implements the state-of-the-art Transformer model as proposed.
* **Key Actions:**
    * Loads the pre-trained `distilbert-base-uncased` model.
    * Tokenizes data with truncation/padding (max length 512).
    * Fine-tunes the model using the Hugging Face `Trainer` API.
    * Evaluates performance against the Baseline.
* **Outputs:** `distilbert_confusion_matrix.png`, `metrics_distilBERT` (logs).

---

##  File Descriptions

### Data
* **`complaints.csv`**: The input dataset from the CFPB. 

### Generated Images
The notebooks automatically generate the following plots used in the final report:
* **`class_imbalance_plot.png`**: Visualization of the `Product` category distribution.
* **`complaints_over_time.png`**: Time-series view of complaint volume.
* **`word_count_by_category.png`**: Boxplot of message lengths per category.
* **`baseline_confusion_matrix.png`**: Error analysis for the Naive Bayes model.
* **`distilbert_confusion_matrix.png`**: Error analysis for the Transformer model.

---

