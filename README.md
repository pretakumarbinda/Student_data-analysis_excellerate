# 📊 Excelerate Opportunity Data Analysis

## 📌 Project Overview
This project focuses on cleaning, validating, and preparing a real-world dataset of user engagement with Excelerate opportunities for further analysis. The dataset contains user demographic information, opportunity details, application timelines, and participation status. The goal is to transform raw, inconsistent data into a clean, structured, and analysis-ready dataset suitable for exploration and insight generation.

This repository documents the complete workflow from raw data to final cleaned output, including feature engineering, validation, and reporting.

---

## 📂 Repository Structure

├── Excelerate_data_analysis.ipynb # Full data cleaning & feature engineering notebook
├── SLU Opportunity Wise Data.csv # Raw dataset
├── cleaned_data.csv # Final cleaned dataset
├── documentation.docx # Project documentation (Word)
├── documentation.pdf # Final report (PDF)
├── README.md # Project overview (this file)


---

## 🛠️ Tools & Technologies
- Python
- Pandas
- NumPy
- Regex (text cleaning)
- Google Colab
- Microsoft Excel (visualization)
- GitHub (version control & sharing)

---

## 🔄 Workflow Summary

### 1️⃣ Data Understanding & Profiling
- Inspected dataset structure, columns, and relationships
- Identified data quality issues such as missing values, malformed dates, inconsistent text, and duplicates
- Analyzed structural missingness in opportunity start dates

---

### 2️⃣ Data Cleaning
The following cleaning steps were performed:

- Removed duplicate application records
- Standardized date formats and removed unnecessary time components
- Fixed inconsistent casing and spelling in text columns
- Normalized institution names using rule-based text cleaning
- Removed location-based variations from institution names
- Cleaned invalid values in names and majors
- Handled multilingual text safely
- Removed low-frequency missing rows
- Dropped redundant highly correlated columns

---

### 3️⃣ Feature Engineering
New features were created to improve analytical value:

- **Age_at_Application_Int** – applicant age at application time
- **Is_Completed** – binary completion indicator
- **Has_Start_Date** – opportunity scheduling indicator
- **Opportunity_Duration_Days** – length of opportunity
- **Institution_Participation_Count** – engagement per institution

These features enable demographic, behavioral, and institutional analysis.

---

### 4️⃣ Data Validation
Validation checks were performed to ensure accuracy and consistency:

- Schema validation (data types)
- Missing value validation (only structural missingness remained)
- Logical date checks (birth < apply < end)
- Duplicate validation (no duplicates remained)
- Feature validation (ranges and binary values verified)

The final dataset is consistent, reliable, and ready for analysis.

---

### 5️⃣ Visualization & Insights
Excel was used to create visualizations showing:
- Opportunity distribution by region
- Gender distribution of participants
- Opportunity distribution by category

These graphs provide high-level insights into participation trends.

---

## 📄 Final Output
- Cleaned and validated dataset
- Fully documented cleaning & feature engineering process
- Engineered features for analysis
- Visual summaries of key patterns
- PDF documentation suitable for submission and portfolio use

---

## 🚀 How to Run This Project

1. Open `Excelerate_data_analysis.ipynb` in Jupyter Notebook or Google Colab
2. Run cells sequentially from top to bottom
3. The cleaned dataset will be generated as `cleaned_data.csv`

---

## 📈 Future Work
- Exploratory data analysis (EDA)
- Engagement trend analysis
- Completion rate analysis
- Demographic insights
- Predictive modeling (optional)

---

## 👤 Author
**Preta Kumar Binda**  
Undergraduate Student | Data Analysis & Machine Learning Enthusiast  
Bangladesh  

---

## ⭐ Notes
This project demonstrates practical data cleaning, feature engineering, and validation techniques applied to a real-world dataset. It is intended for portfolio presentation and learning purposes.
