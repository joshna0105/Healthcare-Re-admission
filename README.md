
# Hospital Readmissions Analysis

## Project Overview
This project analyzes hospital readmissions using patient data. The goal is to understand patterns and trends that lead to patient readmission, including age, hospital stay duration, number of medications, and medical specialties. The analysis is performed using PySpark for data processing and Pandas, Seaborn, and Matplotlib for visualization.

## Dataset
- File: 'data/HospitalReadmissions.csv'
- Description: Contains patient hospitalization records, including numerical and categorical features.
- Key Features: 
  - 'time_in_hospital' – Length of stay in the hospital (days)
  - 'n_lab_procedures' – Number of lab tests performed
  - 'n_procedures' – Number of procedures performed
  - 'n_medications' – Number of medications prescribed
  - 'n_outpatient', 'n_inpatient', 'n_emergency' – Previous hospital visits
  - 'age' – Age group of the patient
  - 'medical_specialty' – Patient's medical specialty
  - 'readmitted' – Whether the patient was readmitted ('yes' or 'no')

## Project Objectives
1. Explore and clean the dataset using PySpark.
2. Perform statistical analysis to calculate counts, averages, and correlations.
3. Visualize key insights using Seaborn and Matplotlib.
4. Provide a summary of trends and patterns to understand readmission risk factors.

## Folder Structure
HospitalReadmissions/
│── Dataset (.csv file)
│── plots/ # Saved charts (optional)
│── HospitalReadmissions_Analytics.ipynb
│── README.md
│── requirements.txt # Python packages

## Libraries Used
- Python 3.x
- Pandas
- Seaborn
- Matplotlib
- PySpark

## How to Run
1. Clone or download this repository.
2. Place the dataset in the 'data/' folder.
3. Open 'HospitalReadmissions_Analytics.ipynb' in Jupyter Notebook.
4. Run all cells sequentially.
5. Visualizations will appear in the notebook. Optionally, they can be saved to the 'plots/' folder.

## Key Visualizations
- Readmission Distribution: Bar chart showing counts of readmitted vs non-readmitted patients.
- Age vs Readmission: Count plot highlighting which age groups have higher readmission rates.
- Hospital Stay Duration vs Readmission: Boxplot showing longer stays are associated with higher readmission.
- Medications Count vs Readmission: Histogram comparing medication counts for readmitted and non-readmitted patients.
- Medical Specialty vs Readmission: Horizontal bar chart showing top 10 specialties with readmission patterns.
- Correlation Heatmap: Heatmap showing correlation between numerical features and readmission.

## Insights
- Elderly patients (ages 70–90) have higher readmission rates.
- Longer hospital stays and higher medication counts are associated with readmission.
- Specialties like Cardiology and Surgery have higher readmission occurrences.
- Numeric features like 'time_in_hospital' and 'n_inpatient' show strong positive correlation with readmission.

## Optional Future Work
- Build predictive models to forecast readmission risk.
- Include more features such as comorbidities and seasonal trends.
- Create interactive dashboards for hospital management.

## Requirements
Install the required Python packages:

```bash
pip install -r requirements.txt
