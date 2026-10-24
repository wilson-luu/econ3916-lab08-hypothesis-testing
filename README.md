# Hypothesis Testing — Is Job Training Worth It?

**Objective:** This project applies one-sample and two-sample t-tests alongside multiple comparison corrections to the LaLonde National Supported Work data to evaluate the statistical and practical significance of a job training program on earnings.

**Methodology:**
* Loaded the LaLonde NSW job training experiment (445 people: 185 trainees and 260 controls).
* Ran a one-sample t-test and a two-sample Welch's t-test on 1978 earnings.
* Wrote Welch's t-statistic as a function, welch_t(), and checked it against scipy on the full sample and on five subgroups.
* Computed Cohen's d, to judge the size of the effect and not only whether it is significant.
* Ran a power analysis: the power of this study, and the sample size needed to detect d = 0.3.
* Tested the treatment effect in 5 overlapping demographic subgroups, then applied Bonferroni and Benjamini-Hochberg corrections.
* Simulated p-value distributions when the null is true and when it is false.

**Key Findings:**
Trainees earned $1794.34 more in 1978 (Welch's t = 2.6741, p = 0.0079), a Cohen's d of 0.2727. 2 of the 5 subgroup effects were significant before correction, and 1 after Bonferroni.
