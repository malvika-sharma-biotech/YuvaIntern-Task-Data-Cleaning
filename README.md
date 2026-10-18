# YuvaIntern-Task-Data-Cleaning
Titanic dataset acquisition, data inspection and preprocessing using Python and Pandas

# YuvaIntern Task 1: Data Acquisition, Cleaning and Preprocessing

## 1. Project Overview
This project focuses on acquiring, inspecting, cleaning, and preprocessing the Titanic passenger dataset using Python and Pandas.

## 2. Objectives
- Acquire a publicly available dataset.
- Inspect dataset structure and data quality.
- Identify missing values and duplicate records.
- Apply appropriate missing-value treatment.
- Export the cleaned dataset for further analysis.

## 3. Tools and Technologies
- Python
- Google Colab
- Pandas
- NumPy
- GitHub

## 4. Dataset
The Titanic dataset was obtained from the public Seaborn data repository.

Source:
https://github.com/mwaskom/seaborn-data/blob/master/titanic.csv

The original dataset contains 891 rows and 15 columns.

## 5. Data Inspection
Initial inspection identified:
- Total rows: 891
- Total columns: 15
- Total missing values: 869
- Duplicate rows flagged initially: 107

Columns with missing values included age, deck, embarked, and embark_town.

## 6. Cleaning and Preprocessing
The following operations were performed:
- Created a separate copy for cleaning.
- Removed the deck column because it contained 688 missing values.
- Filled missing age values using the median.
- Filled missing embarked values using the mode.
- Filled missing embark_town values using the mode.
- Checked missing values and duplicate records after cleaning.

## 7. Results
- Missing values after cleaning: 0
- Duplicate rows flagged after cleaning: 116
- Original dataset preserved separately.
- Cleaned dataset exported as titanic_cleaned.csv.

The increase in flagged duplicate rows requires careful interpretation because removing a column and imputing missing values can make previously different records identical. Duplicate records were not automatically deleted.

## 8. Project Files
- YuvaIntern_Task1_Data_Cleaning.ipynb: Python code and analysis.
- titanic_cleaned.csv: Cleaned dataset.
- titanic_original.csv: Original dataset, if included in the repository.

## 9. Conclusion
This project demonstrates a basic data preprocessing workflow using Python and Pandas. Missing values were handled using median and mode imputation, and the cleaned dataset was exported for further analysis. Duplicate records were identified for additional investigation.

## 10. Reproducibility
Open the Jupyter notebook in Google Colab and run the cells in sequence. The dataset source is provided above.
