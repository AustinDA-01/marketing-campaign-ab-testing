# Marketing Campaign Effectiveness: A/B Testing and Causal Inference Analysis

## Project Overview

Organizations frequently invest in digital advertising campaigns to increase customer engagement and conversions. However, determining whether an advertising campaign actually causes an increase in conversions requires rigorous experimentation and statistical analysis.

This project evaluates the effectiveness of a digital advertising campaign using a randomized A/B test involving 588,101 users. Statistical hypothesis testing and causal inference techniques were used to measure the impact of advertisement exposure on customer conversion behavior.

---

## Business Problem

Did exposure to a digital advertisement increase customer conversion rates compared to a public service announcement (PSA)?

The objective of this analysis was to:

* Evaluate whether advertisement exposure increased conversions.
* Measure the magnitude of the treatment effect.
* Assess statistical significance.
* Quantify uncertainty using confidence intervals.
* Provide a business recommendation regarding campaign deployment.

---

## Dataset

* Total Users: 588,101
* Treatment Group: Advertisement (Ad)
* Control Group: Public Service Announcement (PSA)
* Target Metric: Conversion

### Variables

| Variable      | Description                   |
| ------------- | ----------------------------- |
| user id       | Unique user identifier        |
| test group    | Ad or PSA group               |
| converted     | Whether the user converted    |
| total ads     | Number of ads viewed          |
| most ads day  | Day with highest ad exposure  |
| most ads hour | Hour with highest ad exposure |

---

## Methodology

### Experiment Validation

Verified treatment and control group structure and compared conversion outcomes between groups.

### Statistical Testing

Performed a Chi-Square test of independence to evaluate whether conversion outcomes differed significantly between experimental groups.

### Causal Inference

Estimated:

* Average Treatment Effect (ATE)
* Relative Lift
* 95% Confidence Interval

---

## Key Findings

### Finding #1: Advertisement Exposure Increased Conversion Rates

| Group                     | Conversion Rate |
| ------------------------- | --------------: |
| PSA (Control)             |           1.79% |
| Advertisement (Treatment) |           2.55% |

The advertising treatment produced a 42.9% relative increase in conversions.

---

### Finding #2: Statistically Significant Improvement

Chi-Square Test Results:

* χ² = 54.01
* p < 0.001

The increase in conversions was statistically significant and unlikely to be explained by random variation.

---

### Finding #3: Positive Treatment Effect

Average Treatment Effect (ATE):

0.00769

This indicates that advertisement exposure increased conversion probability by approximately 0.77 percentage points.

95% Confidence Interval:

[0.00595, 0.00943]

Because the entire confidence interval lies above zero, the treatment effect remains statistically significant.

---

## Business Recommendation

The advertising campaign should be deployed to the broader user population.

Supporting evidence:

* Higher conversion rate than control
* Statistically significant treatment effect
* Positive confidence interval bounds
* Meaningful relative lift in conversions

Even small improvements in conversion rates can generate substantial business value when applied across large customer populations.

---

## Technologies Used

* Python
* Pandas
* NumPy
* SciPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## Project Structure

marketing-campaign-ab-testing/

├── Marketing_Campaign_Effectiveness.ipynb

├── README.md

├── requirements.txt

├── conversion_rates.png

├── confidence_interval_plot.png

└── data/

---

## Author

Austin Blunt

MBA, Data Analytics | B.S. Applied Mathematics

Focused on machine learning, experimentation, statistical inference, forecasting, and business analytics.

