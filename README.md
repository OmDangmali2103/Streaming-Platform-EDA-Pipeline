🎬 Disney+ StreamLens — Data Cleaning, Preprocessing & EDA
A streaming-catalog analytics project exploring Disney+ titles, content categories, release trends, genres, and maturity ratings.

Disney+ StreamLens demonstrates a data-analysis workflow that takes a raw content catalogue through data preparation and exploratory analysis, then presents findings in business-friendly outputs. The project brings together Python, SQL, Excel, and Power BI resources to explore the catalogue from multiple analytical perspectives.

🎯 Business Problem
A streaming catalogue contains more than a list of titles. Its metadata can be used to understand the mix of movies and series, the distribution of genres and maturity ratings, and how the catalogue's release years are represented.

This project uses Disney+ catalogue metadata to explore questions such as:
- What types of content appear in the catalogue?
- How is content distributed across genres and maturity ratings?
- What patterns appear across title release years?
- Which data-quality issues need to be addressed before analysis?
- How can cleaned catalogue data be converted into useful summaries and visualisations?
The analysis is descriptive: catalogue metadata can show distributions and associations, but it does not by itself explain viewer preferences, viewing hours, revenue, or business performance.

🧰 Tools & Technologies
Python	Programmatic data inspection, preparation, and exploratory analysis
Pandas	Tabular data manipulation and cleaning
NumPy	Numerical and data-preparation operations, where used
SQL	Structured querying and analysis of catalogue data
Microsoft Excel	Spreadsheet-based examination and analysis
Jupyter Notebook	Interactive, documented analytical workflow


The exact transformations, queries, formulas, and dashboard elements are documented in their respective project files. Only list a tool as a personal skill in a resume if you can explain and demonstrate the work you performed with it.
🔄 Analysis Workflow
Raw Disney+ Catalogue
          │
          ▼
Dataset Inspection & Data-Quality Review
          │
          ▼
Cleaning and Preprocessing
(missing values, consistency, data types)
          │
          ▼
Feature Preparation
          │
          ▼
Exploratory Data Analysis
          │
          ▼
SQL / Excel Analysis 
          │
          ▼
Interpretation of Catalogue Patterns

This diagram represents the overall workflow described by the project. Refer to the project files for the specific steps implemented in each tool.

🧹 Work Completed
1. Data inspection and preparation
The project includes a preprocessing stage intended to make the catalogue more consistent and suitable for analysis. Its scope includes:
- Reviewing the dataset and its fields before analysis.
- Handling missing data as part of data preparation.
- Cleaning and standardising values where needed.
- Preparing fields and derived features for later analysis.
- Making the dataset easier to group, compare, and visualise.
Why it matters: Results from inconsistent or incomplete source data can be misleading. Inspecting data quality before analysis helps make assumptions visible and improves the interpretability of downstream results.
2. Exploratory data analysis (EDA)
The analysis focuses on the following catalogue dimensions:
Analysis area	What it helps examine
Content distribution	The composition of the catalogue, including content categories such as movies and series where represented in the data
Release-year trends	How catalogue titles are distributed across release years
Genres	The genre labels represented in the catalogue and their relative frequency
Maturity ratings	The distribution of content rating categories


These analyses support descriptive comparisons of the catalogue. Numerical totals and rankings should be quoted only from results reproduced from the project files.
3. Multi-tool analysis and presentation
The repository separates work into Python, SQL, Excel, Power_BI, Data, and Presentation folders. This structure makes the different project assets easier to locate and supports examining the same business topic through code, queries, spreadsheets, and visual reporting.

Use each folder's files to verify the specific queries, formulas, charts, and transformations included in your version of the project.
📈 Analytical Outcomes
The project is designed to produce a clearer, analysis-ready view of the Disney+ title catalogue and to organise the investigation into four main outcome areas:
1. Data quality: A documented preprocessing stage for addressing missing or inconsistent catalogue information before using the data for analysis.
2. Catalogue composition: A view of how titles are distributed across available content categories.
3. Temporal patterns: An exploration of how titles are represented across release years.
4. Genre and rating profile: Comparisons of the genre labels and maturity-rating categories present in the catalogue.
What these outcomes can support
- Summarising the composition of a streaming catalogue.
- Comparing the frequency of categories and genre labels.
- Identifying release-year patterns that may warrant further investigation.
- Preparing cleaner, more consistent data for reporting.
- Communicating exploratory findings through tables, charts, and dashboards.
Interpretation note: This dataset describes catalogue metadata. Unless separate viewing or engagement data is included and analysed, it cannot establish which titles are most watched, most profitable, or most preferred by audiences. Correlation or frequency alone should not be described as causation or customer behaviour.
Add verified results here
To make this section stronger for a portfolio review, record the actual outputs produced by your notebook, SQL scripts, Excel analysis, or Power BI report:
- Dataset size: [verified number of rows] rows × [verified number of columns] columns.
- Data-quality checks: [verified number/type of issues found and how they were handled].
- Content mix: [verified count or percentage by content type].
- Genre result: [verified leading genre/category and its count or percentage].
- Release-year result: [verified year or period and the supported observation].
- Rating result: [verified rating distribution observation].
Replace every bracketed field with a result reproduced from the project. Remove any item that the current files do not calculate. Do not leave placeholders in the published README.


🧠 Skills Demonstrated
The project can serve as a practical learning example for:
- Data inspection and data-quality awareness
- Missing-value handling and preprocessing decisions
- Tabular data manipulation with Python and Pandas
- Exploratory data analysis
- Categorical and time-based analysis
- SQL-based querying, where implemented
- Spreadsheet analysis and business reporting
- Communicating findings through visualisation
Be prepared to explain not just the function or tool used, but why a transformation was appropriate, what alternatives existed, and how the result was validated.

⚠️ Limitations
- The analysis is limited to the fields provided in the catalogue dataset.
- Catalogue metadata alone does not measure watch time, audience satisfaction, revenue, or subscriber retention.
- Missing-value treatment may affect interpretation; each treatment should be justified in the corresponding code or documentation.
- Any summary finding should be checked against the underlying data and analysis output before being presented as a factual result.
  
🔭 Possible Improvements
- Add a reproducible run order and a dependency file for the Python workflow.
- Record before-and-after data-quality metrics, such as missing-value counts and duplicate counts.
- Export an explicitly named cleaned dataset while preserving the raw source file.
- Add automated validation checks for expected columns, data types, and key uniqueness assumptions.
- Document the most important SQL queries and explain what each result means.
- Add screenshots of the actual Power BI report and concise explanations of the visuals.
- Include verified quantitative findings in this README instead of broad claims.


This README summarises the project scope and analysis areas described by the repository. Preserve attribution to the original authors, check the source repository's license, and state clearly which changes or extensions you personally implemented.
Project takeaway: StreamLens illustrates how catalogue data can be cleaned, explored, and prepared for reporting. The main deliverable is an analytical workflow for investigating data quality and describing content, release-year, genre, and maturity-rating patterns—not a measurement of actual audience engagement.
