# Healthcare Data Exploratory Data Analysis (EDA)

## Project Overview
This project explores a healthcare dataset using Python. It focuses on understanding patient information, admission patterns, medical conditions, billing amounts, and relationships between numerical variables.

## Objectives
- Inspect the dataset structure and summary statistics.
- Check for missing values and clean selected columns.
- Convert admission and discharge dates to datetime format.
- Calculate the length of each patient's stay.
- Explore admission types, medical conditions, gender, and billing amounts.
- Visualize patterns and relationships in the data.

## Tools and Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## Dataset
The notebook loads a CSV file named `healthcare_data_for_task - healthcare_data_for_task.csv`.

Place the CSV file in the notebook's working directory, or update the file path in the data-loading cell before running the notebook.

The notebook uses fields including:
- `Age`
- `Medical_Code`
- `Admission_Type`
- `Date_of_Admission`
- `Discharge_Date`
- `Billing_Amount`
- `Medical_Condition`
- `Gender`

## Workflow
1. Import the required Python libraries.
2. Load and inspect the dataset using `head()`, `shape`, `info()`, `describe()`, and `columns`.
3. Check missing values and fill missing `Medical_Code` values with `Unknown`.
4. Standardize `Admission_Type` text by trimming spaces and applying title case.
5. Convert admission and discharge dates to datetime values.
6. Calculate `Stay_Days` from discharge date minus admission date.
7. Explore billing statistics, average age by medical condition, and medical-condition counts by gender.
8. Create visualizations:
   - Admission type count bar chart
   - Stacked billing totals by medical condition and admission type
   - <img width="531" height="327" alt="Screenshot 2026-10-14 142614" src="https://github.com/user-attachments/assets/3a76268a-e36c-4a2a-a5a4-1440f0943574" />

   - Billing amount distribution by medical condition (violin plot)
   - <img width="534" height="264" alt="Screenshot 2026-10-14 142652" src="https://github.com/user-attachments/assets/963bcd3e-b910-40e7-b0df-3371a51c761d" />

   - Monthly patient admissions line chart
   - <img width="534" height="227" alt="Screenshot 2026-10-14 142707" src="https://github.com/user-attachments/assets/a51b16ac-86b9-4cdc-a5c2-1eec0dddf0db" />

   - Correlation heatmap for numerical columns
   - <img width="508" height="430" alt="Screenshot 2026-10-14 142730" src="https://github.com/user-attachments/assets/0615b7f5-f276-40e6-843d-e47d47c2d9f1" />

