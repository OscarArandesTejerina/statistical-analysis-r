# Statistical Analysis & Visualization in R

Two independent statistical analyses conducted in R, applying hypothesis testing and data visualization to real-world datasets. The focus throughout is on appropriate test selection, checking the assumptions behind each test, and communicating results clearly, rather than simply running functions and reporting p-values.

## Overview

The project is split into two parts, each built around a set of research questions:

**Part 1 — Bank Marketing.** An analysis of customer data from a Portuguese bank's direct marketing campaign (2008–2010) aimed at encouraging clients to subscribe to a term deposit. Two questions are addressed:

- Is there a correlation between a customer's age and their bank balance?
- Is there an association between a client's marital status and term deposit subscription?

**Part 2 — Sleep Health & Lifestyle.** An exploration of how lifestyle factors relate to sleep health, using a dataset covering age, gender, occupation, sleep quality, BMI, and sleep disorders. Two questions are addressed:

- Is there a significant difference in sleep duration between male and female participants?
- Does sleep quality differ across BMI categories or across sleep disorders?

## Methods

The analysis demonstrates a range of statistical techniques and, importantly, the reasoning behind choosing each one:

- **Correlation** — Pearson vs. Spearman, selected based on whether linearity and normality assumptions hold.
- **Association testing** — Chi-square test for association on contingency tables, with residual analysis to interpret which cells drive the result.
- **Group comparisons** — two-sample t-test and one-way ANOVA, with non-parametric alternatives (Wilcoxon rank-sum, Kruskal-Wallis) used when assumptions are violated.
- **Assumption checking** — histograms, Q-Q plots, residuals-vs-fitted plots, and the Shapiro-Wilk test for normality.
- **Post-hoc analysis** — pairwise Wilcoxon tests with Holm's correction and the Nemenyi all-pairs test for multiple comparisons.
- **Visualization** — scatter plots, bar plots, boxplots, and diagnostic plots to support each conclusion.

## Key Findings

- **Age and balance** show no meaningful correlation.
- **Marital status is significantly associated with term deposit subscription**, with single customers subscribing more often than expected and married customers less often.
- **Sleep duration differs significantly by gender**, with females sleeping longer on average.
- **Sleep quality differs across BMI categories and across sleep disorders**, with the clearest differences between overweight and normal groups, and between the insomnia and none groups.

## Datasets

- Bank marketing data (via Kaggle, originally from Moro et al.).
- Sleep Health and Lifestyle dataset (Kaggle) — a synthetic dataset used for illustrative purposes.

Both sources are cited in full in the report.

## Repository Contents

```
statistical-analysis-r/
├── README.md
├── report/          # Full write-up (PDF) with methods, results, and discussion
├── src/             # R scripts for each research question
└── figures/         # Generated plots
```

## Tech

R · statistical hypothesis testing · non-parametric methods · data visualization

## Report

The full report, including detailed methodology, results tables, and discussion, is available in the `report/` folder.
