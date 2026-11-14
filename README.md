
<div align="center">

# Food Delivery Data Analysis

### From Raw Delivery Records to Reliable, Data-Driven Insights

A Python-based data analytics project focused on data understanding, quality assessment, and cleaning of food delivery operational data.

<br>

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

![Project Status](https://img.shields.io/badge/Status-Week%201%20Completed-success?style=flat-square)
![Records](https://img.shields.io/badge/Records-45%2C584-blue?style=flat-square)
![Columns](https://img.shields.io/badge/Columns-20-informational?style=flat-square)

</div>

---

## 1. Project Overview

Food delivery platforms generate large volumes of operational data every day. This data contains valuable information about orders, delivery personnel, restaurants, traffic conditions, weather, and delivery duration.

However, raw datasets often contain missing values, inconsistent formats, and other data-quality issues that can affect the reliability of analysis.

This project focuses on understanding, inspecting, and cleaning a food delivery dataset containing **45,584 records and 20 columns**.

The primary objective is to transform raw delivery records into a structured, analysis-ready dataset while documenting every important cleaning decision.

## 2. Project Objectives

- Understand the structure and characteristics of the dataset.
- Identify missing values and duplicate records.
- Inspect numerical and categorical variables.
- Validate date and time information.
- Detect inconsistent time formats.
- Apply appropriate data-cleaning techniques.
- Maintain a detailed cleaning log.
- Export and verify the cleaned dataset.

## 3. Dataset Information

| Attribute | Details |
|---|---|
| Dataset Name | Food Delivery Dataset |
| Total Records | 45,584 |
| Total Columns | 20 |
| File Format | CSV |
| Data Type | Structured Tabular Data |
| Domain | Food Delivery Operations |
| Primary Tools | Python, Pandas, NumPy |

### Key Dataset Features

The dataset contains information related to:

- Delivery personnel age and ratings
- Restaurant and delivery location coordinates
- Order dates and timings
- Weather conditions
- Road traffic density
- Vehicle conditions and types
- Order categories
- Festival information
- Delivery duration

## 4. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Data processing and analysis |
| Pandas | Data manipulation and cleaning |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Jupyter Notebook | Interactive analysis and documentation |

## 5. Project Workflow

### 5.1 Data Understanding

- Loaded and inspected the original dataset.
- Examined dataset dimensions, column names, and data types.
- Used statistical summaries to understand numerical variables.
- Inspected categorical values and distributions.

### 5.2 Data Quality Assessment

Performed systematic checks for:

- Missing values across columns.
- Duplicate rows and duplicate IDs.
- Unusual numerical observations.
- Categorical value inconsistencies.
- Invalid date and time formats.

### 5.3 Data Cleaning

The following cleaning operations were performed:

| Data Quality Issue | Cleaning Approach |
|---|---|
| Missing delivery age | Median imputation |
| Missing delivery ratings | Median imputation |
| Missing delivery count | Median imputation |
| Missing categorical values | Replaced with `Unknown` |
| Decimal-based time values | Converted to HH:MM format |
| Selected pickup times beyond midnight | Normalized to next-day clock time |
| Missing order times | Retained without guessing |

Unusual numerical values were inspected and retained where their meaning could not be confirmed from the available dataset documentation.

### 5.4 Validation and Export

- Compared original and cleaned dataset dimensions.
- Verified duplicate records after cleaning.
- Reviewed remaining missing values.
- Exported the cleaned dataset as a CSV file.
- Reloaded the exported file to validate its structure.
- Maintained a separate cleaning log.

## 6. Key Results

The cleaning process produced the following results:

| Metric | Result |
|---|---:|
| Original Records | 45,584 |
| Cleaned Records | 45,584 |
| Total Columns | 20 |
| Rows Removed | 0 |
| Duplicate Rows | 0 |
| Cleaning Log Entries | 16 |
| Remaining Missing Values | 1,731 |

### Data Quality Note

The remaining 1,731 missing values belong to the `Time_Orderd` column.

These values were intentionally retained because their actual order times could not be reliably determined. This avoids introducing unsupported assumptions into the dataset.

## 7. Repository Structure

```text
food-delivery-data-analysis/
│
├── data/
│   ├── raw/
│   │   └── README.md
│   │
│   └── processed/
│       └── cleaned_food_delivery.csv
│
├── notebooks/
│   └── 01_data_understanding_and_cleaning.ipynb
│
├── docs/
│   └── cleaning_log.csv
│
├── README.md
└── requirements.txt
```

## 8. Installation and Setup

Follow these steps to run the project locally.

### Step 1: Clone the Repository

```bash
git clone https://github.com/ayushi857-dev/food-delivery-data-analysis.git
```

### Step 2: Navigate to the Project Directory

```bash
cd food-delivery-data-analysis
```

### Step 3: Install Dependencies

```bash
pip install -r requirements.txt
```

### Step 4: Launch Jupyter Notebook

```bash
jupyter notebook
```

Open the following notebook:

`notebooks/01_data_understanding_and_cleaning.ipynb`

### Dataset Access

The original dataset is required to execute the notebook from scratch.

Place the CSV file at:

`data/raw/Food delivery Dataset.csv`

Refer to `data/raw/README.md` for dataset access instructions.

## 9. Project Deliverables

- Data understanding and inspection notebook.
- Data quality assessment.
- Cleaned food delivery dataset.
- Documented cleaning log.
- Final validation and export verification.

## 10. Learning Outcomes

Through this project, I gained practical experience in:

- Working with real-world structured datasets.
- Identifying and handling missing data.
- Applying Pandas data-cleaning techniques.
- Inspecting numerical and categorical variables.
- Validating date and time formats.
- Documenting analytical decisions.
- Building reproducible data preparation workflows.

## 11. Future Scope

The cleaned dataset can be used for further analysis, including:

- Exploratory Data Analysis (EDA).
- Delivery-time distribution analysis.
- Impact of weather on delivery duration.
- Relationship between traffic density and delivery time.
- City-wise operational comparisons.
- Data visualization and business insight generation.

## 12. Author

**Ayushi Shukla**

Aspiring Data Analyst | AI/ML Enthusiast

- GitHub: [ayushi857-dev](https://github.com/ayushi857-dev)
- Project Repository: [Food Delivery Data Analysis](https://github.com/ayushi857-dev/food-delivery-data-analysis)

---

<div align="center">

**Built with Python, curiosity, and a data-driven mindset.**

</div>
