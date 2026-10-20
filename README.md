# 🎓 Learning and Quality Performance Analytics

### 📊 End-to-End Excel Data Processing & Power BI Business Intelligence Project

**From raw practice data to validated datasets, interactive dashboards, and business-focused insights.**

---

## 🌟 1. Project Overview

**Learning and Quality Performance Analytics** is an independent portfolio project that explores employee training performance, assessment outcomes, and quality audit results using Microsoft Excel and Power BI.

The project simulates an analytical workflow for a Learning & Quality (L&Q) team. It demonstrates how structured data can be reviewed, cleaned, validated, modeled, and transformed into interactive reports that help managers understand performance and investigate opportunities for improvement.

The project was developed in two main stages:

- 🟢 **Stage 1 — Excel:** Data processing, cleaning, validation, reconciliation, and preliminary KPI analysis.
- 🔵 **Stage 2 — Power BI:** Data modeling, DAX measures, interactive visualizations, dashboard development, and target-based scenario analysis.

🎯 **Main objective:** Build a reliable, business-oriented reporting solution that connects data quality with learning performance and quality analysis.

> This is a practice project built with practice data. It is not an official company dashboard and does not represent verified internal company performance.

---

## 🏢 2. Business Problem

Organizations that deliver employee training need to understand whether training is being completed, how employees perform in assessments, and where operational quality issues may require attention.

Simply reporting training completion is not enough. Decision-makers also need to investigate assessment outcomes, training timeliness, department-level patterns, and potential improvement opportunities.

This project addresses these needs through a three-page Power BI dashboard.

### 🎯 Business objectives

- Monitor training assignment status and completion.
- Evaluate training completion timeliness.
- Analyze assessment pass rates and score distributions.
- Compare assessment and quality performance across departments.
- Examine quality audit records by error category.
- Explore assessment outcomes by course and attempt number.
- Calculate the additional assessment passes needed to reach a selected target.
- Communicate findings and data-quality limitations transparently.

---

## ❓ 3. Business Questions Answered

### 📚 Page 1 — Learning Performance Overview

**Primary business question:** How effectively is the organization managing and completing assigned training?

| Business question | Dashboard analysis |
|---|---|
| How much training has been assigned? | Total training assignments KPI |
| How many assignments are completed or pending? | Training assignment status chart and KPI cards |
| What proportion of training assignments is completed? | Training completion rate |
| How does training completion vary by department? | Training completion rate by department |
| Are completed assignments on time or late? | Training completion timeliness donut chart |
| How does the volume of training assignments change over time? | Monthly training assignment trend |

**Business value:** Helps managers understand training workload, completion patterns, timeliness, and areas that may need follow-up.

### ⭐ Page 2 — Quality & Performance Analysis

**Primary business question:** How are employees performing in assessments, and where might quality issues need attention?

| Business question | Dashboard analysis |
|---|---|
| What proportion of assessment records has a passing result? | Assessment pass rate KPI |
| How are assessment scores distributed? | Assessment score distribution |
| How do average assessment and quality scores vary by department? | Assessment and quality performance matrix |
| Which quality error categories account for more audit records? | Quality audit records by error category treemap |
| How can users explore assessment performance for a specific course? | Course slicer |

**Business value:** Helps users explore assessment performance and quality audit patterns, identify areas for investigation, and support further analysis.

### 🚀 Page 3 — Training Effectiveness & Action Plan

**Primary business question:** Where should the organization focus its training efforts to improve assessment performance?

| Business question | Dashboard analysis |
|---|---|
| How many assessment records have a failing result? | Assessment fail count KPI |
| How many distinct employee IDs have assessment records? | Employees assessed KPI |
| What is the current assessment pass rate? | Current assessment pass rate KPI |
| How do pass and fail counts compare across courses? | Assessment outcomes by course |
| How do average scores vary across recorded attempt numbers? | Average assessment score by attempt |
| How many additional passes are needed to reach a selected target? | Interactive target pass-rate scenario |
| What is the gap between the current pass rate and the selected target? | Pass rate improvement gap |
| What actions could be considered based on the results? | Training Improvement Action Center |

**Business value:** Extends descriptive reporting with a what-if scenario that quantifies the number of additional passing assessment records needed to reach a chosen target.

---

## 🛠️ 4. Tools and Technologies

| Tool | How it was used |
|---|---|
| 🟢 Microsoft Excel | Data review, cleaning, validation, formulas, reconciliation, and KPI analysis |
| 🔵 Microsoft Power BI | Data modeling, interactive reports, and visual analytics |
| 🧮 DAX | Measures, calculated columns, and dynamic target-based calculations |
| 🔗 Power BI relationships | Connected employee and trainer reference tables to relevant analytical tables |
| 🎛️ Power BI slicers | Enabled interactive filtering and target selection |
| 📝 GitHub | Project documentation, repository management, and portfolio presentation |

---

## 🗃️ 5. Dataset Overview

The cleaned practice workbook contains five main analytical tables.

| Dataset | Cleaned record count | Purpose |
|---|---:|---|
| 👥 Employees | 2,500 | Employee attributes and department analysis |
| 📚 Training | 12,000 | Assignment status, assigned dates, due dates, completion dates, and training hours |
| 📝 Assessments | 9,000 | Assessment scores, recorded outcomes, courses, and attempt numbers |
| 🔍 Quality Audits | 15,000 | Quality scores, audit dates, error categories, and processes |
| 🧑‍🏫 Trainers | 35 | Trainer reference information |

These are the record counts used during the project. The datasets are for practice and portfolio demonstration, not verified company records.

---

## 🔄 6. End-to-End Project Workflow

### 🟢 Stage 1 — Excel Data Processing and Validation

**Objective:** Prepare the datasets and document their quality before analysis in Power BI.

#### Step 1: Inspect the source data
- Reviewed the available worksheets and their column structures.
- Identified the employee, training, assessment, quality audit, and trainer datasets.
- Preserved the original raw sheets while working with cleaned versions.

#### Step 2: Clean and validate the datasets
- Identified duplicate records and removed duplicates from the cleaned datasets.
- Checked missing values in important columns.
- Reviewed training assignment, due, and completion dates.
- Checked assessment and quality scores against the valid 0–100 range.
- Validated employee and trainer references.
- Reviewed status counts and reconciled totals.

#### Step 3: Prepare KPI analysis
- Calculated training assignment and completion metrics.
- Calculated assessment pass counts and pass rate.
- Calculated preliminary average assessment and quality scores.
- Documented validation results and known limitations.

**Excel output:** A prepared workbook with cleaned datasets, validation results, a data dictionary, and KPI analysis.

### 🔵 Stage 2 — Power BI Data Modeling and Dashboard Development

**Objective:** Turn the prepared Excel data into an interactive business intelligence report.

#### Step 1: Import the cleaned tables
Imported the five cleaned datasets into Power BI using the Excel workbook as the data source.

#### Step 2: Establish relationships
Created active relationships between:

- `Clean_Employees` and `Clean_Training`
- `Clean_Employees` and `Clean_Assessments`
- `Clean_Employees` and `Clean_Quality_Audits`
- `Clean_Trainers` and `Clean_Training`

The relationships support employee- and trainer-related filtering and analysis.

#### Step 3: Develop DAX measures
Created measures for training assignments, completed assignments, completion rate, status counts, assessment pass count, assessment pass rate, average scores, and quality audit metrics.

#### Step 4: Build the dashboards
Developed three pages with distinct business purposes:

1. 📚 Learning Performance Overview
2. ⭐ Quality & Performance Analysis
3. 🚀 Training Effectiveness & Action Plan

#### Step 5: Add interactive analysis
Implemented a What-if parameter that lets a user select an assessment pass-rate target and view the additional passes needed to reach it.

#### Step 6: Review the results
Checked KPI values against the practice workbook and documented known data-quality limitations.

### 🔁 Workflow summary

**Excel source data → Data cleaning and validation → KPI analysis → Power BI data modeling → DAX measures → Interactive dashboards → Business interpretation**

---

## 🧪 7. Data Quality Issues Encountered and How They Were Handled

Data quality was a major part of the project. The following issues were identified during Excel validation and Power BI development.

### 🔁 Issue 1 — Duplicate records

**Problem:** Duplicate rows were present in the source datasets.

**Handling:** Duplicate records were identified and removed from the cleaned datasets. The raw sheets were preserved for reference.

**Result:** The cleaned tables used in the project contain the record counts documented above.

### 🕳️ Issue 2 — Missing values

**Problem:** Some employee and training fields contained missing values, including location, joining date, employee ID, due date, and completion date.

**Handling:** Missing values were reviewed and documented. They were not automatically replaced with invented values simply to make the validation indicators appear complete.

**Important limitation:** Some missing values remain in the prepared datasets. A missing value is not automatically an error that should be deleted; the correct handling depends on the business meaning of the field.

### 📅 Issue 3 — Inconsistent training dates

**Problem:** Some training records had completion dates before their assigned dates.

**Finding:** 407 training records were identified with completion dates earlier than assignment dates.

**Handling:** These records were identified during validation and represented as `Invalid Date` in the training timeliness classification.

**Important limitation:** Classification makes the issue visible; it does not correct the underlying dates.

### 📝 Issue 4 — Assessment scores outside the valid range

**Problem:** Assessment scores are expected to fall between 0 and 100, but some records fell outside that range.

**Finding:** 45 invalid assessment scores were identified, with observed values ranging from -5 to 120.

**Handling:** The assessment score distribution visual filters scores to the 0–100 range. However, the preliminary average assessment score measure includes the invalid values.

**Improvement opportunity:** Create a valid-score-only measure and investigate the source of invalid records before using the average for formal performance decisions.

### 🔍 Issue 5 — Quality scores outside the valid range

**Problem:** Some quality audit scores were outside the expected 0–100 range.

**Finding:** 60 invalid quality scores were identified, with observed values ranging from -10 to 150.

**Handling:** Invalid values were documented through validation. The preliminary average quality score currently includes them.

**Improvement opportunity:** Create a valid-score-only quality measure and investigate the invalid records.

### 🔗 Issue 6 — Unmatched employee references

**Problem:** Some assessment and quality audit records contained employee IDs that did not match the employee reference table.

**Findings:**
- Assessments: 20 unmatched employee references.
- Quality audits: 30 unmatched employee references.

**Handling:** These records were identified during validation and documented as data-quality issues.

**Important limitation:** The unmatched references were not confirmed as corrected. They should be investigated before relying on employee-level reporting as a complete representation of the employee population.

### 🧮 Issue 7 — Reconciling training counts

**Problem:** Training status counts and missing-value totals needed to be reconciled after duplicate removal and cleaning.

**Handling:** Training status counts were checked against the cleaned assignment total of 12,000 records. Missing-value counts were reconciled across the relevant training fields.

**Result:** The recorded status counts sum to the cleaned training assignment total.

### 🎛️ Issue 8 — Building a dynamic target scenario

**Problem:** The report needed to show more than current performance. It needed to let a manager explore a potential target.

**Solution:** Created a What-if parameter named `Target Pass Rate`, along with DAX measures for additional passes needed and the pass-rate improvement gap.

**Result:** The scenario updates when the target changes, while keeping the total number of assessment records fixed.

---

## 📌 8. Key Performance Indicators

The following results come from the practice dataset and the KPI calculations performed during the project.

| KPI | Result |
|---|---:|
| 📚 Total training assignments | 12,000 |
| ✅ Completed training assignments | 7,935 |
| 🎯 Training completion rate | 66.13% |
| ⏳ Pending training assignments | 25 |
| 🔄 In-progress training assignments | 1,672 |
| 📝 Total assessment records | 9,000 |
| 🟢 Assessment pass count | 3,506 |
| 🎯 Assessment pass rate | 38.96% |
| 📊 Average assessment score | 75.68 — preliminary |
| 🔍 Total quality audit records | 15,000 |
| 📈 Average quality score | 83.65 — preliminary |
| ✅ Quality score validity rate | 99.60% |

**Interpretation notes:**

- The training completion rate is based on completed assignments divided by total training assignments.
- The assessment pass rate is based on recorded pass outcomes divided by total assessment records.
- The average assessment and quality scores are preliminary because invalid scores remain included in the current average measures.
- The quality score validity rate represents the proportion of quality audit records with scores between 0 and 100.

These values describe the practice dataset and should not be presented as verified findings about a real organization.

---

## 🎛️ 9. Interactive What-if Analysis

The third dashboard page includes an interactive target pass-rate scenario.

### Example: Target pass rate of 50%

| Calculation | Value |
|---|---:|
| Total assessment records | 9,000 |
| Current passing records | 3,506 |
| Selected target | 50% |
| Passing records required | 4,500 |
| Additional passing records required | 994 |
| Current pass rate | 38.96% |
| Gap to target | 11.04 percentage points |

The calculation is:

**Additional passes needed = MAX(0, required passes − current passes)**

For a 50% target:

- Required passing records = 9,000 × 50% = 4,500.
- Additional passing records = 4,500 − 3,506 = 994.
- Improvement gap = 50.00% − 38.96% = 11.04 percentage points.

This scenario assumes that the assessment record count remains fixed at 9,000.

**Important:** This is a mathematical planning scenario, not a prediction that training interventions will automatically produce 994 additional passes.

---

## 💡 10. Business Insights and Potential Actions

The dashboards support the following types of business interpretation.

### 📚 Training management
The 66.13% training completion rate indicates that a substantial proportion of assignments were not recorded as completed in the practice dataset. Managers could investigate outstanding assignments, due dates, and department-level differences.

### 📝 Assessment performance
The 38.96% assessment pass rate highlights an opportunity to investigate assessment outcomes. Course-level comparisons can help identify where further review may be useful.

### 🔍 Quality monitoring
The quality audit error-category treemap supports investigation of categories with higher record counts. High counts indicate more recorded audit entries in a category, not necessarily a higher error rate, because category-specific denominators and exposure levels may differ.

### 🎯 Improvement planning
The target pass-rate scenario quantifies the number of additional passing assessment records required for a selected target. This gives managers a clear numerical goal to evaluate alongside potential learning interventions.

These are potential interpretations and follow-up actions, not proof that a particular course, department, or employee is responsible for a business problem.

---

## 🎨 11. Dashboard Design Principles

The dashboard was designed around the following principles:

- 🎯 **Business purpose:** Each visual addresses a defined business question.
- 📊 **Appropriate visual selection:** Charts and matrices are chosen to support the relevant analysis.
- 🔁 **Avoid duplication:** The three pages focus on different aspects of learning and quality performance.
- 👁️ **Visual hierarchy:** KPI cards and page titles help establish context.
- 🎨 **Consistent styling:** A coordinated orange background with navy and teal accents is used across pages.
- 🎛️ **Interactive analysis:** Slicers and the target scenario support exploration.
- ⚠️ **Data transparency:** Known quality limitations are documented instead of being silently ignored.
- 💼 **Portfolio presentation:** The report is structured to demonstrate practical analytical skills.

---

## 🖼️ 12. Dashboard Preview

The following images will display once the corresponding screenshots have been uploaded to the repository.

### 📚 Learning Performance Overview

![Learning Performance Overview](screenshots/learning-performance-overview.png)

### ⭐ Quality & Performance Analysis

![Quality & Performance Analysis](screenshots/quality-performance-analysis.png)

### 🚀 Training Effectiveness & Action Plan

![Training Effectiveness & Action Plan](screenshots/training-effectiveness-action-plan.png)

---

## 📁 13. Repository Contents

The repository is intended to include:

- 📗 Excel practice workbook containing the prepared datasets and validation analysis.
- 📊 Power BI report (`.pbix`) containing the three dashboard pages.
- 🖼️ Dashboard screenshots.
- 🎥 Combined dashboard demonstration video.
- 📝 This README and supporting project documentation.

The repository contents will depend on which files have been uploaded and committed.

---

## 🚀 14. Future Improvements

Potential next steps include:

- 🧹 Create valid-score-only measures for assessment and quality averages.
- 🔗 Investigate and resolve unmatched employee references.
- 📅 Review invalid training dates and determine the appropriate corrections.
- 📚 Explore course-level assessment outcomes in greater detail.
- 📊 Add more robust data-quality checks and a documented validation process.
- 🎯 Expand the interactive improvement scenario with clearly defined assumptions.
- 🔄 Explore a repeatable refresh process for updated Excel data.
- 📝 Document the measures, relationships, and business definitions used in the report.

---

## 👨‍💻 15. Skills Demonstrated

- Microsoft Excel data processing and validation
- Missing-value and duplicate analysis
- Data-quality checks and reconciliation
- KPI calculation and interpretation
- Power BI data modeling and relationships
- DAX measures and calculated columns
- Interactive dashboard development
- Business-focused data visualization
- What-if scenario analysis
- Technical documentation and GitHub portfolio management

---

## ⚖️ 16. Project Disclaimer

This is an independent portfolio practice project built with practice data. It is not an official company dashboard and does not represent verified internal company data, employee performance, or operational results from any real organization.

The findings and potential actions documented here are limited to the available practice dataset and the assumptions described in this README.

---

## ⭐ Conclusion

Learning and Quality Performance Analytics demonstrates an end-to-end analytical workflow, beginning with **Excel data processing and validation** and continuing through **Power BI data modeling, DAX calculations, interactive dashboards, and business interpretation**.

The project emphasizes that effective analytics requires more than attractive visuals: it also requires reliable data, clearly defined metrics, appropriate business questions, and transparent communication of limitations.

Thank you for exploring this project! 🚀
