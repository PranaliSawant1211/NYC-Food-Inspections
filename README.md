# NYC Food Inspections – Data Preparation & Modeling Project

## 🧼 Project Overview

This project focuses on preparing and analyzing restaurant inspection data from New York City to evaluate food safety compliance. Using a combination of **SQL**, **Alteryx**, and **data modeling techniques**, the project transforms raw public health data into a clean, reliable dataset ready for insights and visualization.

The pipeline supports robust data profiling, preparation, and normalization to assist health authorities and data analysts in identifying hygiene trends, risky establishments, and inspection score patterns across NYC.

---

## 🗃️ Dataset Details

- **Source**: [NYC Open Data - Restaurant Inspection Results](https://data.cityofnewyork.us/Health/DOHMH-New-York-City-Restaurant-Inspection-Results/43nn-pn8j)
- **Records Processed**: ~500K+
- **Dataset Name**: *DOHMH_New_York_City_Restaurant_Inspection_Results*
- **Key Columns**:
  - `CAMIS` (Establishment ID), `DBA` (Restaurant Name), `BORO`, `ZIPCODE`
  - `INSPECTION DATE`, `SCORE`, `GRADE`
  - `VIOLATION CODE`, `VIOLATION DESCRIPTION`
  - `CUISINE DESCRIPTION`, `INSPECTION TYPE`

---

## 🎯 Project Goals

- Clean and standardize half a million restaurant inspection records.
- Perform deep **data profiling** to detect nulls, inconsistencies, and duplicates.
- Normalize and transform the data using **Alteryx workflows**.
- Implement a **SQL-based physical data model** to support downstream querying.
- Lay the groundwork for building business intelligence dashboards.

---

## 🛠️ Tools & Technologies

- **Alteryx Designer** – Data profiling, transformation, and workflow automation.
- **SQL (T-SQL / MySQL syntax)** – Schema creation, data prep, and normalization.
- **ER Modeling (via .sql)** – Physical data model creation for normalized reporting.
- **Microsoft Word** – Project documentation.
- **GitHub** – Source control and project collaboration.

---

## 📁 Repository Structure

| File | Description |
|------|-------------|
| `DOHMH_New_York_City_Restaurant_Inspection...csv` | Raw NYC inspection dataset file. |
| `Food_inspections_NYC.sql` | SQL script for preparing the cleaned inspection table. |
| `NYCFoodInspection_DataPreparation.yxmd` | Main Alteryx workflow for transforming inspection data. |
| `NYCFoodInspection_DataProfiling.yxmd` | Alteryx workflow used for profiling and assessing data quality. |
| `NYCNewWorkflow.yxmd` | Additional data prep or transformation logic (support workflow). |
| `NYC_Food_Establishment_PhysicalDataModel.sql` | Physical data model schema including primary/foreign keys and normalized tables. |
| `NYC_foodInspection_DataPrep.sql` | SQL queries used to clean and enrich the raw dataset. |
| `.bak` Files | Backup versions of Alteryx workflows for redundancy. |
| `NYC_FoodInspection.docx` | Word doc with project documentation or key summary points. |

---

## 🔍 Data Profiling Highlights

- Identified nulls and inconsistent formatting across inspection and violation codes.
- Standardized date formats and resolved mixed-case and inconsistent cuisine descriptions.
- Removed exact duplicate inspections to ensure clean aggregation of scores.
- Validated ZIP codes and borough relationships for geolocation accuracy.

---

## 📐 Data Modeling Summary

- Created a **normalized physical schema** to support relational queries.
- Key entities modeled:
  - `Restaurant`
  - `Inspection`
  - `Violation`
  - `Location`
  - `Cuisine`
- Linked with appropriate **primary and foreign keys** to maintain referential integrity.

---

## 📈 Use Cases & Impact

- **Health Department Insights**: Prioritize follow-up inspections for high-risk establishments.
- **Geographic Analysis**: Map hygiene violations by borough and ZIP code.
- **Trend Analysis**: Visualize changes in inspection scores and grades over time.
- **Dashboard Integration**: Structure data to support tools like Power BI or Tableau.

---

## 💡 Skills Demonstrated

- Data Cleaning & Transformation (SQL + Alteryx)
- Data Profiling & Quality Checks
- Physical Schema Design & Normalization
- Workflow Automation and ETL Documentation
- Git/GitHub Collaboration

---

## 🚀 Future Enhancements

- Connect data to Tableau for dashboard reporting.
- Add temporal aggregation by quarter/month for trend analysis.
- Create summary reports for top violations by cuisine or borough.
- Integrate real-time updates using NYC’s public API (if available).

---

## 🙋‍♀️ Author

**Pranali Sawant**  
📫 [LinkedIn](https://www.linkedin.com/in/pranalisawantt12/) | 📧 pranalisawantt12@gmail.com  
🔬 Passionate about building clean data pipelines to solve real-world problems in public health and compliance.

---

## 📜 License

This project is open-source and available under the [MIT License](LICENSE).

---

⭐ If this project helped or inspired you, give it a ⭐ and feel free to connect with me!
