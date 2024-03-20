# Job Title Prediction Project

## Introduction
This project aims to develop a predictive model that accurately determines a job's title based on its description and other related fields. The goal is to enhance the job matching algorithm's accuracy and performance at a career services company, Y.

## Problem Statement
The objective is to analyze job descriptions, required skills, and other provided fields to predict the job title accurately. This is an open-ended task allowing for creativity and expertise in data science to approach the problem effectively.

## Expectations
We value not only a high-performing model but also a demonstration of a research mindset, curiosity about data, and fit with our collaborative culture in data science. The process, explorations, and findings should be presented with the standards upheld in the data science community.

## Data Sets
- **job_data.csv**: Contains fields such as function, job_title, and jds (job descriptions).
  - The function field categorizes the job into broader segments like IT, Sales, etc.
  - The job_title is the target variable.
  - The jds field contains detailed job descriptions, including experience requirements, skills, and other job-related information.

## Tasks
1. **Data Preprocessing**: Clean and prepare the data for modeling. This includes handling missing values, encoding categorical variables, and parsing text data to extract features.
2. **Feature Engineering**: Derive meaningful features from the job descriptions and other fields that could be predictive of the job title.
3. **Modeling**: Experiment with different machine learning algorithms to predict job titles.
4. **Validation**: Validate the model's performance using appropriate metrics and validation techniques. Discuss the choice of metrics.
5. **Documentation**: Document findings, challenges, assumptions, insights on feature importance, and model interpretability.

## Repository Structure
- **data**: Contains the dataset(s) used in the project.
- **notebooks**: Jupyter notebooks for data exploration, preprocessing, modeling, and evaluation.
- **scripts**: Python scripts for data preprocessing, feature engineering, and modeling.
- **reports**: Documentation, including a comprehensive report of findings, challenges, assumptions, and insights.
- **README.md**: Overview of the project, instructions, and key information.

## Techniques Used
- **Data Preprocessing**:
' Handling Missing Values: Missing values in the 'jds' field were handled using the SimpleImputer from scikit-learn, replacing them with the most frequent value.
' Removing Duplicates: Duplicates in the dataset were identified and removed using the drop_duplicates method in pandas.
' Text Data Cleaning: Text data in the job descriptions ('jds') was preprocessed to remove punctuation, tokenize, and perform stopword removal using the Natural Language Toolkit (NLTK) library. This involved lowercasing, removing punctuation, tokenizing, stopword removal, and either stemming or lemmatization.

- **Feature Engineering**:
' TF-IDF Vectorization: The job descriptions were transformed into numerical feature vectors using TF-IDF (Term Frequency-Inverse Document Frequency) vectorization. This technique assigns weights to words based on their frequency in the document and inverse frequency across all documents, capturing their importance.
' Word Cloud Visualization: Word clouds were generated to visually represent the most frequent words in the job titles, functions, and descriptions, providing insights into the dataset's textual data distribution.

- **Modeling**:
' Random Forest Classifier: A Random Forest Classifier was chosen as the initial model for predicting job titles. This ensemble learning method combines multiple decision trees to improve performance and reduce overfitting. It was trained on the TF-IDF features extracted from the job descriptions.

- **Evaluation**:
' Accuracy Score: The accuracy score was used to evaluate the model's performance on the test data, measuring the proportion of correctly predicted job titles.
' F1 Score: The F1 score, which is the harmonic mean of precision and recall, was also calculated to assess the model's overall performance, especially in handling class imbalances.
' Classification Report: The classification report provided detailed metrics such as precision, recall, and F1-score for each class, offering insights into the model's performance across different job titles.

' These techniques were chosen and implemented to preprocess the data effectively, engineer meaningful features, build predictive models, and evaluate their performance accurately. They collectively contribute to developing a robust job title prediction system.


## Usage
1. Clone the repository: `git clone https://github.com/Pradhyumn1/spectra_assign.git`
2. Navigate to the project directory: `cd job_title_prediction`
3. Set up the environment: `pip install -r requirements.txt`
4. Run the notebooks/scripts for data preprocessing, modeling, and evaluation.
5. Refer to the documentation in the reports folder for detailed insights and findings.

## Contributors
- [Your Name](https://github.com/Pradhyumn1)

