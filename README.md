# Healthcare Analysis

## Hospital Operations & Patient Experience Analytics

An end-to-end healthcare analytics project using Python, Pandas, NumPy, Matplotlib, and SciPy to analyze hospital operations, patient experience, and billing data.

## Business Goal

This project analyzes:

- Patient demographics and hospital visits
- Department workload and waiting times
- Patient satisfaction
- Insurance and payment patterns
- High-demand periods
- Areas where hospital operations can be improved

## Dataset

The project uses three related datasets:

- `patients.csv` — patient details such as age, gender, city, BMI, chronic condition, and insurance status.
- `visits.csv` — department, diagnosis, visit type, waiting time, satisfaction score, and length of stay.
- `billing.csv` — bill amount, insurance coverage, patient-paid amount, payment method, and payment status.

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- SciPy
- Jupyter Notebook

## Project Workflow

### 1. Data Understanding

- Loaded Patients, Visits, and Billing datasets.
- Checked data types, missing values, duplicates, and data structure.

### 2. Data Cleaning

The project uses business-rule-based data cleaning, including:

- Removing duplicate records
- Standardizing categorical values
- Handling invalid ages and BMI values
- Converting numeric and date columns
- Filling missing values using group-based patterns
- Handling missing insurance and billing information
- Calculating missing patient-paid amounts

### 3. Data Integration

The Patients, Visits, and Billing datasets were merged to create a combined analytical dataset, using Visits as the main transaction table.

### 4. Feature Engineering

Created features such as:

- Age group
- Visit day and month
- Visit time band
- Out-of-pocket percentage
- High-wait flag
- Repeat-patient flag
- Waiting-time bands

## Analysis Performed

### Univariate Analysis

- Visits by age group
- Chronic conditions
- Insurance mix
- Waiting-time distribution
- Visits by city

### Bivariate Analysis

- Waiting time by department
- Visit volume by department
- Waiting time vs. satisfaction
- Out-of-pocket payment by insurance group
- Billing by visit type
- Age group and chronic conditions

### Multivariate & Diagnostic Analysis

- Department and visit-type waiting times
- Peak demand by day and hour
- Repeat-patient utilization
- Satisfaction difference between low-wait and high-wait patients

A t-test was used to evaluate the satisfaction difference between low-wait and high-wait groups.

## Key Findings

- The **46–60 age group** has the highest number of visits.
- **Hypertension** is the most frequent chronic condition when patients without a chronic condition are excluded.
- **Insured** patients represent about **49.9%** of visits.
- Average waiting time is about **45.4 minutes**, with approximately **15.2%** of visits waiting over 60 minutes.
- **Hyderabad** contributes the highest number of visits.
- **Cardiology** has the highest average waiting time at about **58.9 minutes**.
- **General Medicine** has the highest visit volume.
- Patient satisfaction decreases as waiting time increases.
- **Self-pay** patients have the highest average out-of-pocket share.
- **Inpatient** visits have the highest average bill, approximately **₹28,641**.
- **Cardiology OPD** has an average waiting time of around **61.6 minutes**.
- The busiest day is **Wednesday**, with the busiest hour around **13:00**.
- The notebook reports a statistically significant satisfaction difference between low-wait and high-wait patients (**p < 0.001**).

## Business Recommendations

### 1. Improve Cardiology OPD Flow
Review doctor scheduling, appointment slots, and registration processes.

### 2. Monitor Waiting-Time KPIs
Track average waiting time, median waiting time, and visits waiting over 60 minutes.

### 3. Align Staffing With Demand
Use peak day and hourly patterns to improve staff planning.

### 4. Improve Chronic-Care Follow-Up
Create focused follow-up workflows for high-utilization patient groups.

### 5. Support Self-Pay Patients
Improve cost communication and payment options for patients with higher out-of-pocket expenses.

### 6. Monitor Patient Experience
Track patient satisfaction together with waiting-time performance.

## Project Structure

```text
Healthcare-Analysis/
│
├── Healthcare_Analysis.ipynb
├── patients.csv
├── visits.csv
├── billing.csv
└── README.md
```

> If the CSV files are not included in the repository, update the notebook's data-loading paths before sharing the project.

## How to Run

1. Install Python and Jupyter Notebook.
2. Install the required libraries:

```bash
pip install pandas numpy matplotlib scipy
```

3. Place the notebook and CSV files in the appropriate folders.
4. Open `Healthcare_Analysis.ipynb`.
5. Run the notebook cells from top to bottom.

## Project Approach

**Business Question → Data Understanding → Data Cleaning → Data Integration → Feature Engineering → Analysis → Visualization → Insight → Recommendation**

This project demonstrates practical skills in data cleaning, analysis, visualization, statistical analysis, and business insight generation.

## Author

**Mrudula Potpillewar**

BCA Graduate | MCA Student | Data Analytics & AI Learner

**Skills:** Python, Pandas, NumPy, SQL, Excel, Data Visualization, Healthcare Data Analysis
