# 🎬 StreamLens
### Data Cleaning, Preprocessing & Exploratory Data Analysis

Transforming raw streaming-platform data into structured, analysis-ready information and meaningful insights.

---

## 📌 Project Overview

Raw datasets are rarely ready for analysis. Missing values, inconsistent text, incorrect data types, duplicate records, and poorly formatted dates can reduce data quality and lead to misleading conclusions.

**Disney+ StreamLens** explores a Disney+ streaming catalogue dataset through data cleaning, preprocessing, and exploratory data analysis (EDA). The objective is to transform raw catalogue information into a more consistent and reliable dataset, then investigate patterns in content types, genres, release years, ratings, and other available attributes.

The project follows an important analytics principle:

> **Reliable insights begin with reliable data.**

Rather than jumping directly into visualizations, the workflow emphasizes understanding the data, identifying quality issues, making appropriate cleaning decisions, and validating the resulting dataset before drawing conclusions.

## 🎯 Business Problem

Streaming platforms offer large and diverse content catalogues. Analyzing this information can help answer questions about the composition of a catalogue, the distribution of content across genres, and changes in release patterns over time.

This project investigates the following questions:

- What types of content are represented in the dataset?
- How is content distributed across genres?
- What patterns can be observed in release years?
- How are ratings and other categorical attributes distributed?
- Which data-quality issues must be addressed before analysis?
- How can the cleaned dataset support reliable downstream reporting?

These are exploratory questions. The dataset alone does not establish viewership, audience engagement, popularity, or business performance.

---

## 🔄 Project Workflow

```text
Raw Disney+ Catalogue Dataset
             │
             ▼
      Data Inspection
             │
             ▼
   Data Quality Assessment
             │
             ▼
     Data Cleaning
             │
             ▼
  Type Conversion & Standardization
             │
             ▼
    Data Validation
             │
             ▼
 Exploratory Data Analysis (EDA)
             │
             ▼
  Visualizations & Findings
             │
             ▼
   Analysis-Ready Dataset
```

## 🧹 1. Data Cleaning & Preprocessing

The first stage focuses on identifying and addressing data-quality issues before performing exploratory analysis.

### Data inspection
- Examine the dataset's structure, columns, and data types.
- Inspect missing values and duplicate records.
- Identify inconsistent or incorrectly formatted values.
- Review date-related columns and categorical attributes.

### Data cleaning
- **Missing values:** Assess null values and apply appropriate handling based on the affected column.
- **Duplicate records:** Check for duplicate entries and remove them where appropriate.
- **Date formatting:** Convert valid date values into suitable datetime formats where required.
- **Text standardization:** Improve consistency in categorical text values.
- **Data types:** Ensure columns use appropriate types for analysis.
- **Data validation:** Check the cleaned data for remaining inconsistencies and unexpected values.

Cleaning decisions should preserve meaningful information. Missing values are not automatically errors, and duplicate-looking records should be investigated before removal.

## 🐍 2. Python-Based Data Analysis

Python provides the primary environment for working with the dataset.

| Library | Purpose |
|---|---|
| **Pandas** | Data inspection, filtering, cleaning, transformation, and aggregation |
| **NumPy** | Numerical operations and analytical support |
| **Matplotlib** | Creating charts and visual representations |
| **Seaborn** | Statistical visualization and distribution analysis |

The workflow separates data preparation from exploratory analysis so that visualizations are based on a consistent dataset.

## 📊 3. Exploratory Data Analysis

After preparing the data, EDA is used to understand its structure and investigate patterns in the streaming catalogue.

### Content type analysis

Examine the distribution of available content types, such as movies and television shows, where those categories exist in the dataset.

**Analytical purpose:** Understand the composition of the catalogue and compare the relative representation of content types.

### Genre analysis

Explore genre categories and their representation across the catalogue.

**Analytical purpose:** Identify commonly represented genres and understand how catalogue content is distributed across classifications.

### Release-year analysis

Investigate the distribution of release years and changes in the number of catalogue entries across different periods.

**Analytical purpose:** Understand the historical release profile of the available content.

### Ratings analysis

Examine the distribution of content ratings and identify the categories represented in the dataset.

**Analytical purpose:** Understand the catalogue's content-rating composition. Content ratings should not be interpreted as audience satisfaction or viewer scores.

### Data-quality analysis

Inspect missing values, duplicates, data types, and categorical consistency before and after cleaning.

**Analytical purpose:** Establish whether the dataset is sufficiently consistent for the intended analysis and identify limitations that should be documented.

---

## 💡 4. Project Outcomes & Business Interpretation

The project is designed to deliver outcomes at two levels: **improved data readiness** and **better understanding of the catalogue**.

### Outcome 1 — A more analysis-ready dataset

Data cleaning and preprocessing help standardize the dataset's structure, improve consistency, and reduce avoidable data-quality problems.

**Why it matters:** Reliable downstream analysis depends on using appropriate data types, understanding missing values, and applying consistent transformations.

### Outcome 2 — A clearer picture of catalogue composition

Content-type and genre analysis provide a structured view of how the catalogue is represented.

**Why it matters:** Such analysis can help catalogue analysts describe the available content and identify areas worth investigating further.

### Outcome 3 — Better understanding of release patterns

Analyzing release-year distributions helps reveal how catalogue entries are spread across time periods.

**Why it matters:** This can support descriptive reporting about catalogue composition, although release dates alone cannot establish why content was added or how well it performed.

### Outcome 4 — More informed interpretation of ratings

Examining rating categories helps describe the maturity classifications represented in the dataset.

**Why it matters:** It enables a more accurate understanding of the catalogue's classification profile without confusing content ratings with audience reviews.

### Outcome 5 — A reproducible analytical foundation

Separating inspection, cleaning, validation, and EDA creates a workflow that can be reviewed and repeated.

**Why it matters:** A documented workflow is easier to debug, maintain, extend, and reuse when working with updated datasets.

> **Results transparency:** Numerical findings—such as the number of rows cleaned, missing values resolved, content-type percentages, most common genres, and release-year trends—should be added after checking the actual notebook outputs. No numerical outcomes are claimed here without verification.

---

## 🧠 5. Skills Demonstrated

This project provides practical exposure to:

- Python for data analysis
- Data wrangling using Pandas and NumPy
- Missing-value and duplicate assessment
- Date and data-type handling
- Categorical data standardization
- Data-quality validation
- Exploratory data analysis
- Statistical and categorical visualization
- Analytical reasoning and interpretation
- Documenting data preparation decisions

The emphasis is on understanding why a transformation is needed, not simply applying a function to the dataset.

*The structure above summarizes the repository's main areas. Consult the actual folders for their specific files and implementation details.*

## 🚀 6. How to Explore the Project

### Prerequisites

- Python 3
- Jupyter Notebook or VS Code with notebook support
- pandas
- numpy
- matplotlib
- seaborn

### Steps

1. Clone or download the repository.
2. Open the Python analysis files in VS Code or Jupyter Notebook.
3. Install the required Python libraries in your environment.
4. Review the raw dataset and the documented data-quality issues.
5. Execute the analysis in the intended order, starting with inspection and cleaning.
6. Review the resulting visualizations and validate the findings against the data.

Additional tools included in the repository may require their own setup and should be explored according to the files provided.

## ⚠️ 7. Limitations & Responsible Interpretation

- Findings describe the dataset being analyzed; they do not automatically generalize to all streaming platforms.
- Catalogue data does not, by itself, establish viewing behavior, customer preferences, engagement, or revenue.
- Cleaning decisions can affect analytical results and should be documented.
- Correlation or co-occurrence should not be interpreted as causation.
- Numerical claims should be traceable to reproducible calculations.

## 🔮 8. Potential Improvements

Possible future enhancements include:

- Add automated data-quality checks and a before-and-after cleaning summary.
- Create a repeatable preprocessing script that exports a validated, cleaned CSV.
- Add verified numerical findings and supporting visualizations.
- Introduce logging and exception handling for more robust data preparation.
- Add automated tests for critical cleaning rules.
- Document how the workflow can be rerun when the source dataset changes.

These are potential extensions, not claims about features already implemented.

---

## 📌 Conclusion

**StreamLens** demonstrates the importance of data preparation as a foundation for analytics. By combining data inspection, cleaning, validation, and exploratory analysis, the project establishes a structured approach to turning raw catalogue data into information that can be interpreted more reliably.

Its core value is not simply producing charts—it is making the data more consistent, understanding its limitations, and using evidence to describe patterns in the catalogue.

