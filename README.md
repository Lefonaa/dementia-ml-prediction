# Dementia Risk Classification & Predictive Modeling

## Project Overview
This project focuses on the development of a machine learning model to classify dementia risk using a clinical dataset of **2,149 patients**. As a 3rd-year Data Science student, I utilized this project to master the end-to-end ML pipeline, with a specific focus on complex data preprocessing and feature engineering for healthcare applications.

## Technical Stack
* **Language:** Python
* **Environment:** Jupyter Notebook
* **Libraries:** Pandas (Data Wrangling), NumPy (Numerical Analysis), Matplotlib/Seaborn (Visualization), Scikit-learn (Machine Learning)

## Data Preprocessing & Cleaning
Healthcare data requires rigorous cleaning to ensure model reliability.
* **Indexing:** Assigned `PatientID` as the unique index to ensure data integrity.
* **Handling Missing Values:** Implemented `health.dropna()` to remove incomplete records, ensuring a high-quality training set.
* **Feature Management:** Removed non-predictive columns like `Unnamed: 0` to reduce model noise.



## Advanced Feature Engineering
This project served as a deep dive into transforming raw clinical data into model-ready features:

### 1. Categorical Encoding
To handle various categorical data types, I implemented three distinct strategies based on feature characteristics:
* **One-Hot Encoding:** Used for nominal data like `Gender` or `Ethnicity`.
* **Ordinal Encoding:** Applied to ranked categories like `EducationLevel`.
* **Binary Encoding:** Implemented for high-cardinality features to optimize memory and model performance.

### 2. Feature Standardization
I applied scaling to numerical variables (Age, BMI, AlcoholConsumption) to ensure the model isn't biased by different units of measurement. This transforms the data into a standard normal distribution where:
$$\mu = 0, \sigma = 1$$



### 3. Feature Selection
Focused on identifying the most statistically significant predictors, such as `MemoryComplaints` and `BehavioralProblems`, to improve the predictive power and interpretability of the model.

## Model Training & Evaluation
The model was trained to distinguish between dementia risk levels based on clinical markers.
* **Evaluation Metrics:** Performance was measured using **Accuracy**, **Precision**, and **Recall** to account for the high stakes of medical classification.
* **Fairness:** I prioritized ensuring the model performed consistently across different demographic groups, aligning with my core research interests in **algorithmic fairness**.



## Key Learning Outcomes
* Mastered the implementation of multiple encoding strategies within a single pipeline.
* Gained practical experience in **Feature Standardization** and **Selection** to optimize model performance.
* Developed a deeper understanding of how critical data cleaning decisions impact clinical classification results.

---
**Author:** Lefona Moloi
**Education:** BSc Information Technology (Data Science) | Eduvos
