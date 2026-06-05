# A/B Testing & Experimentation Analytics Platform

## 1. Project Overview

A/B Testing & Experimentation Analytics Platform is an end-to-end Product Analytics and Statistical Experimentation solution developed using Python, Pandas, SciPy, Statsmodels, and Matplotlib.

The project simulates and evaluates A/B experiments to determine whether a new product or website variant leads to a statistically significant improvement in business performance. It combines data generation, exploratory data analysis, hypothesis testing, confidence interval estimation, statistical power analysis, sample size estimation, and revenue impact modeling.

The platform enables organizations to make data-driven product decisions by identifying winning variants and quantifying their business impact.

---

## 2. Business Problem

Organizations frequently introduce new website designs, product features, marketing campaigns, and user experiences to improve customer engagement and conversion rates.

Without proper experimentation and statistical validation, it becomes difficult to:

* Determine whether a new variant actually improves performance.
* Distinguish real improvements from random fluctuations.
* Estimate the financial impact of a change.
* Calculate required sample sizes before launching experiments.
* Evaluate whether experimental results are trustworthy.
* Make confident business decisions based on data.

This project addresses these challenges by implementing a complete experimentation analytics workflow used by modern product and analytics teams.

---

## 3. Project Objectives

* Simulate realistic A/B testing datasets.
* Analyze conversion rate performance across variants.
* Perform statistical hypothesis testing.
* Calculate confidence intervals for conversion rates.
* Conduct statistical power analysis.
* Estimate required sample sizes for experiments.
* Quantify revenue impact of winning variants.
* Generate actionable business recommendations.

---

## 4. Dataset

The project uses a simulated A/B testing dataset generated using Python.

Dataset Characteristics:

* 10,000 Users
* Two Experimental Groups (A and B)
* Conversion Events
* Simulated Website/Product Variants

Generated Dataset:

* ab_test_data.csv

Dataset Structure:

| Column    | Description              |
| --------- | ------------------------ |
| user_id   | Unique user identifier   |
| group     | Experimental group (A/B) |
| converted | Conversion outcome (0/1) |

---

## 5. Technology Stack

### Programming & Analytics

* Python
* Pandas
* NumPy

### Statistical Analysis

* SciPy
* Statsmodels

### Visualization

* Matplotlib

### Analytics Techniques

* A/B Testing
* Hypothesis Testing
* Conversion Rate Analysis
* Confidence Interval Estimation
* Statistical Power Analysis
* Sample Size Calculation
* Revenue Impact Analysis

---

## 6. Setup and Execution

### Prerequisites

Install the following:

* Python 3.x

### Install Required Python Packages

```bash
pip install pandas numpy matplotlib scipy statsmodels
```

---

## 7. Running the Project

### Step 1: Generate A/B Testing Dataset

```bash
python src/data_generator.py
```

Generated File:

* ab_test_data.csv

---

### Step 2: Perform Exploratory Data Analysis

```bash
python src/eda.py
```

Provides:

* Dataset Summary
* Group Distribution
* Conversion Distribution
* Conversion Rate Analysis

---

### Step 3: Perform Statistical Hypothesis Testing

```bash
python src/statistical_testing.py
```

Provides:

* Z-Test
* P-Value Analysis
* Statistical Significance Evaluation

---

### Step 4: Calculate Revenue Impact

```bash
python src/revenue_impact.py
```

Provides:

* Additional Monthly Conversions
* Monthly Revenue Uplift
* Annual Revenue Uplift

Results:

* Estimated Annual Revenue Gain: $1.76 Million

---

### Step 5: Calculate Confidence Intervals

```bash
python src/confidence_intervals.py
```

Provides:

* Conversion Rate Confidence Intervals
* Statistical Reliability Assessment

Results:

* Group A: 4.93%

* 95% CI: [4.33%, 5.53%]

* Group B: 6.40%

* 95% CI: [5.72%, 7.08%]

---

### Step 6: Perform Statistical Power Analysis

```bash
python src/power_analysis.py
```

Provides:

* Effect Size Calculation
* Statistical Power Estimation

Results:

* Statistical Power: 88.98%
* Experiment Sufficiently Powered

---

### Step 7: Calculate Required Sample Size

```bash
python src/sample_size_calculator.py
```

Provides:

* Minimum Required Users per Group
* Total Required Experiment Size

Results:

* Required Users per Group: 3,765
* Total Users Required: 7,531

---

## 8. Project Workflow

### Data Generation

A realistic A/B testing dataset was generated using probabilistic simulation.

Groups:

* Variant A (Control)
* Variant B (Treatment)

---

### Exploratory Data Analysis

Analyzed:

* User Distribution
* Conversion Counts
* Conversion Rates

Results:

* Group A Conversion Rate: 4.93%
* Group B Conversion Rate: 6.40%

---

### Hypothesis Testing

Performed a two-proportion Z-Test to determine whether the observed difference was statistically significant.

Results:

* Z-Statistic: -3.1795
* P-Value: 0.0015

Conclusion:

* Variant B significantly outperformed Variant A.

---

### Confidence Interval Analysis

Estimated 95% confidence intervals for conversion rates.

This provided a range of plausible values for the true conversion rate of each variant.

---

### Statistical Power Analysis

Evaluated whether the experiment contained sufficient users to detect the observed effect.

Result:

* Statistical Power: 88.98%

---

### Revenue Impact Modeling

Estimated business impact based on:

* Monthly Visitors
* Average Order Value
* Conversion Rate Improvement

Results:

* Monthly Revenue Gain: $146,944
* Annual Revenue Gain: $1.76 Million

---

### Sample Size Estimation

Calculated the required sample size needed to reliably detect the observed conversion improvement.

Result:

* 3,765 Users per Group

---

## 9. Key Insights

* Variant B achieved a significantly higher conversion rate.
* The observed improvement was statistically significant.
* The experiment achieved sufficient statistical power.
* Confidence intervals support the superiority of Variant B.
* Deploying Variant B could generate substantial revenue growth.
* Proper sample size planning is critical for reliable experimentation.

---

## 10. Business Recommendations

* Deploy Variant B as the production version.
* Continue monitoring conversion performance post-deployment.
* Use sample size calculations before future experiments.
* Establish experimentation frameworks for feature releases.
* Quantify business impact alongside statistical significance.
* Implement continuous product experimentation for optimization.

---

## 11. Project Structure

AB_Testing_Platform/

├── data/

│   └── ab_test_data.csv

├── notebooks/

├── outputs/

├── src/

│   ├── data_generator.py

│   ├── eda.py

│   ├── statistical_testing.py

│   ├── confidence_intervals.py

│   ├── power_analysis.py

│   └── sample_size_calculator.py

├── requirements.txt

└── README.md

---

## 12. Key Results

### Conversion Performance

| Group | Conversion Rate |
| ----- | --------------- |
| A     | 4.93%           |
| B     | 6.40%           |

---

### Statistical Significance

| Metric      | Value   |
| ----------- | ------- |
| Z-Statistic | -3.1795 |
| P-Value     | 0.0015  |

Result:

* Statistically Significant Improvement

---

### Revenue Impact

| Metric               | Value      |
| -------------------- | ---------- |
| Monthly Revenue Gain | $146,944   |
| Annual Revenue Gain  | $1,763,330 |

---

### Experiment Quality

| Metric                   | Value  |
| ------------------------ | ------ |
| Statistical Power        | 88.98% |
| Required Users per Group | 3,765  |

---

## 13. Future Improvements

* Bayesian A/B Testing
* Multi-Variant Testing (A/B/n)
* Sequential Testing
* Streamlit Web Application
* Automated Experiment Reports
* Real-Time Experiment Monitoring
* Revenue Forecasting Models
* Experiment Tracking Dashboard

---

## 14. Author

**David Birru**

B.Tech Biotechnology
Indian Institute of Technology Kharagpur

Skills:

* Python
* Pandas
* NumPy
* Statistics
* Hypothesis Testing
* Product Analytics
* Business Analytics
* Experimentation Analytics

GitHub: https://github.com/Davidbirru
