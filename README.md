# Student Performance Analysis: Data Cleaning and Exploratory Data Analysis

**Project Type:** Data Analytics Case Study  
**Organization:** EduPulse Analytics (Case Study)  
**Role:** Junior Data Analyst  
**Tools:** Python, Pandas, Jupyter Notebook, Matplotlib/Seaborn

## 1. Project Overview

This project explores student performance data to understand academic outcomes, identify data quality issues, and investigate the relationship between attendance and examination marks.

The case study simulates a data analytics task at EduPulse Analytics, where the objective is to prepare student records for analysis and extract insights that could help educational institutions make data-informed decisions.

The notebook demonstrates fundamental data analysis techniques, including data inspection, missing-value treatment, duplicate removal, outlier handling, feature engineering, descriptive statistics, and data visualization.

## 2. Business Problem

EduPulse University is concerned about student academic performance and wants to understand the factors associated with student outcomes.

The analysis focuses on the following questions:

- What is the average student mark?
- How many students scored above 75 marks?
- Is attendance associated with examination performance?
- How many students pass or fail based on a defined threshold?
- Are missing values and duplicate records affecting data quality?
- Are there invalid attendance percentages or unusual age and marks values?
- How can the dataset be prepared for reliable reporting?

## 3. Project Objectives

1. Inspect the structure and quality of the student dataset.
2. Calculate descriptive statistics for relevant numerical columns.
3. Identify and handle missing values.
4. Detect and remove duplicate records.
5. Correct invalid or implausible values using appropriate cleaning rules.
6. Create a pass/fail feature using a defined marks threshold.
7. Analyze the relationship between attendance and marks.
8. Visualize the distribution of student marks.
9. Prepare a cleaner dataset for further analysis.

## 4. Technologies Used

| Technology | Purpose |
|---|---|
| Python | Programming and analysis |
| Pandas | Data manipulation and cleaning |
| Jupyter Notebook | Interactive analysis |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Google Colab | Optional cloud-based notebook execution |

## 5. Dataset Description

The notebook references a student performance dataset containing fields such as:

| Column | Description |
|---|---|
| Name | Student name or identifier |
| Age | Student age |
| Marks | Examination marks |
| Attendance_Percentage | Student attendance percentage |

The dataset is intended to contain imperfect records for practicing data cleaning.

**Important:** Confirm the actual column names, number of records, data types, and dataset source before publishing final dataset statistics. No numerical findings are claimed in this README until the notebook has been executed successfully against the actual CSV file.

## 6. Methodology

### Step 1: Data Inspection

Use Pandas to load the dataset and inspect its structure.

Typical operations include:

- Displaying the first and last rows.
- Reviewing column data types.
- Generating descriptive statistics.
- Checking the number of records and columns.

### Step 2: Missing-Value Analysis

Identify missing values using `isnull()` and `isnull().sum()`.

Possible treatments include:

- Imputing missing numerical values when justified.
- Assigning a missing-category label where appropriate.
- Removing records only when justified by the analysis.

The treatment should depend on the extent of missing data and the meaning of the affected field.

### Step 3: Duplicate Removal

Identify repeated records using `duplicated()` and remove confirmed duplicates where appropriate.

This helps prevent repeated records from distorting summary statistics.

### Step 4: Data Quality Corrections

Inspect values that violate expected data rules.

Examples include:

- Attendance percentages above 100%.
- Negative examination marks.
- Implausible ages.

Corrections should be based on documented assumptions, valid ranges, or source verification rather than automatically replacing every unusual value with a mean.

### Step 5: Feature Engineering

Create a binary `Pass` column using the case study's specified threshold:

- `True` when marks are greater than or equal to 50.
- `False` when marks are below 50.

This feature supports a basic summary of pass and fail outcomes.

### Step 6: Descriptive and Correlation Analysis

Calculate the average marks and count students scoring above 75.

Calculate the correlation coefficient between attendance and marks to examine the direction and strength of their linear association.

Correlation does not establish causation.

### Step 7: Visualization

Create a histogram of student marks to examine their distribution.

A professional visualization should include:

- A descriptive title.
- Clearly labelled axes.
- Readable formatting.
- An optional grid where useful.

## 7. Expected Deliverables

The project aims to produce:

- A structured analysis notebook.
- A documented data-cleaning workflow.
- A cleaned dataset, if saved as an output.
- Summary statistics for marks and student outcomes.
- An attendance-versus-marks correlation result.
- A histogram showing the distribution of marks.
- Recommendations for improving data quality and further analysis.

These are intended deliverables; confirm that each has been generated before describing it as completed.

## 8. How to Run the Project

### Option A: Google Colab

1. Open [Google Colab](https://colab.research.google.com/).
2. Upload `Case_Study_Student.ipynb`.
3. Upload the required CSV dataset.
4. Update the file-loading path if necessary.
5. Run the notebook cells in order.

### Option B: Run Locally

Clone the repository:

```bash
git clone https://github.com/YOUR-USERNAME/student-performance-analysis.git
```

Move into the project folder:

```bash
cd student-performance-analysis
```

Install the dependencies:

```bash
python -m pip install -r requirements.txt
```

Start Jupyter Notebook:

```bash
jupyter notebook
```

Open `Case_Study_Student.ipynb` and execute the cells in sequence.

Replace `YOUR-USERNAME` with your GitHub username.

## 9. Key Skills Demonstrated

- Python programming fundamentals.
- Data inspection and descriptive statistics.
- Data cleaning and preprocessing.
- Missing-value and duplicate handling.
- Basic feature engineering.
- Correlation analysis.
- Data visualization.
- Translating a business problem into analytical questions.
- Documenting assumptions and analytical workflows.

## 10. Limitations

This is a foundational case study and should not be treated as a complete educational research study.

Potential limitations include:

- Dataset size and representativeness may be limited.
- Mean imputation can affect the distribution of numerical data.
- Correlation does not establish a causal relationship.
- Pass/fail thresholds depend on the case study's assumptions.
- Data-cleaning decisions can influence analytical findings.

Actual limitations should be updated after inspecting the dataset and running the complete analysis.

## 11. Future Improvements

Potential extensions include:

- Compare attendance patterns across performance groups.
- Examine the distribution of marks using box plots and histograms.
- Analyze pass rates and average marks by relevant student groups.
- Add data validation checks and a reproducible cleaning pipeline.
- Build an interactive dashboard using Streamlit or Power BI.
- Explore predictive modeling only after assessing data quality and suitability.

## 12. Conclusion

This case study provides practical experience in preparing student performance data for analysis. It combines basic Python programming with data quality checks, descriptive statistics, feature engineering, and visualization.

The project establishes a foundation for more advanced educational analytics and demonstrates how structured data analysis can help identify patterns requiring further investigation.

---

**Author:** Your Name  
**Project:** Student Performance Analysis  
**Repository:** Add your GitHub repository URL after publishing.
