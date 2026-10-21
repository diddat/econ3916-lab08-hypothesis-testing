# econ3916-lab08-hypothesis-testing

Hypothesis Testing — Is Job Training Worth It?
Objective
I tested whether job training increased earnings and explored how effect sizes, sample sizes, and multiple testing affect the conclusions.
Methodology
- I loaded the LaLonde NSW experiment with 445 people: 185 trainees and 260 controls.
- I compared earnings distributions and ran a one-sample t-test and a two-sample Welch's t-test.
- I wrote welch_t() and checked it against scipy for the full sample and five subgroups.
- I calculated Cohen's d and used power analysis to examine the study's power and the sample size needed to detect d = 0.3.
- I tested five overlapping demographic subgroups and applied Bonferroni and Benjamini-Hochberg corrections.
- I simulated p-values with and without real effects and examined false findings among significant results.
Key Findings
Trainees earned $1,794.34 more on average in 1978. Welch's t-statistic was 2.6741, with p = 0.0079. Cohen's d was 0.2727, a small standardized effect. Two of the five subgroup effects were significant before correction, and one remained significant after Bonferroni correction. The same subgroup remained significant after Benjamini-Hochberg correction. The earnings difference supports a positive training effect, but deciding whether to fund the program also requires information about its costs and how long the benefits last.
