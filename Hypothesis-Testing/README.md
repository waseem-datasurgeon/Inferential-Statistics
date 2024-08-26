# Hypothesis Testing

## 1. **Introduction to Hypothesis Testing**

Hypothesis testing is a statistical method used to make decisions about a population parameter based on sample data. It involves making an initial assumption (the null hypothesis) and testing whether the observed data provides sufficient evidence to reject this assumption.

## 2. **Key Concepts**

- **Null Hypothesis (H₀)**: A statement of no effect or no difference. It is the hypothesis that the test seeks to disprove.
- **Alternative Hypothesis (H₁ or Ha)**: A statement that contradicts the null hypothesis. It represents the effect or difference that the test aims to detect.
- **Significance Level (α)**: The probability of rejecting the null hypothesis when it is true. Commonly used values are 0.05, 0.01, and 0.10.
- **Test Statistic**: A standardized value calculated from sample data, used to determine whether to reject the null hypothesis.
- **P-value**: The probability of obtaining a test statistic as extreme as, or more extreme than, the observed value, assuming the null hypothesis is true.
- **Decision Rule**: A criterion for rejecting or failing to reject the null hypothesis, based on the significance level and the p-value.

## 3. **Steps in Hypothesis Testing**

1. **State the Hypotheses**: Formulate the null and alternative hypotheses.
    - Example: H₀: μ = 100 (population mean is 100)
    H₁: μ ≠ 100 (population mean is not 100)
2. **Choose the Significance Level (α)**: Select the probability threshold for rejecting the null hypothesis (e.g., α = 0.05).
3. **Collect and Summarize the Data**: Obtain sample data and compute relevant statistics (e.g., sample mean, standard deviation).
4. **Calculate the Test Statistic**: Compute the test statistic based on the sample data and the type of test.
    - Example: For a Z-test, calculate Z = (X̄ - μ) / (σ/√n), where X̄ is the sample mean, μ is the population mean, σ is the population standard deviation, and n is the sample size.
5. **Determine the P-value or Critical Value**: Find the p-value corresponding to the test statistic, or compare the test statistic to the critical value from the relevant distribution.
6. **Make a Decision**: Based on the p-value and the significance level, decide whether to reject or fail to reject the null hypothesis.
    - If p-value ≤ α, reject H₀.
    - If p-value > α, fail to reject H₀.
7. **Interpret the Results**: Draw conclusions in the context of the research question.

## 4. **Types of Tests**

### **Z-test**

- **Purpose**: Test the mean of a sample against a known population mean.
- **Conditions**: Large sample size (n > 30), known population variance.
- **Formula**:  $( Z = \frac{X̄ - μ}{\frac{σ}{√n}} )$
- **Example**: Testing if the average height of students in a school is different from the national average height.

### **T-test**

- **Purpose**: Test the mean(s) when population variance is unknown.
- **Types**:
    - **One-sample T-test**: Compare the sample mean to a known value.
        - **Formula**: $( T = \frac{X̄ - μ}{\frac{s}{√n}} )$, where $s$ is the sample standard deviation.
    - **Independent two-sample T-test**: Compare means of two independent samples.
        - **Formula**:  $( T = \frac{(X̄_1 - X̄_2)}{\sqrt{(\frac{s_1^2}{n_1}) + (\frac{s_2^2}{n_2})}} )$
    - **Paired T-test**: Compare means of two related samples.
        - **Formula**: $( T = \frac{D̄}{\frac{s_D}{√n}} )$, where $D̄$ is the mean of differences, and $s_D$ is the standard deviation of differences.

### **Chi-square test**

- **Purpose**: Test the association between categorical variables.
- **Types**:
    - **Chi-square goodness of fit**: Compare observed frequencies to expected frequencies.
        - **Formula**: \( χ² = \sum \frac{(O_i - E_i)^2}{E_i} \), where O_i is observed frequency, and E_i is expected frequency.
    - **Chi-square test of independence**: Test if two categorical variables are independent.
        - **Formula**: Same as goodness of fit, but applied to contingency tables.

### **ANOVA (Analysis of Variance)**

- **Purpose**: Compare means of three or more groups.
- **Types**:
    - **One-way ANOVA**: Test differences based on one factor.
        - **Formula**: \( F = \frac{MS_{between}}{MS_{within}} \), where MS is mean square.
    - **Two-way ANOVA**: Test differences based on two factors.
- **Conditions**: Normally distributed populations, equal variances, independent samples.

### **Non-parametric Tests**

- **Mann-Whitney U Test**: Compare two independent samples (alternative to independent T-test).
    - **Conditions**: Non-normal data, ordinal data.
- **Wilcoxon Signed-Rank Test**: Compare two related samples (alternative to paired T-test).
    - **Conditions**: Non-normal data, ordinal data.
- **Kruskal-Wallis H Test**: Compare three or more groups (alternative to one-way ANOVA).
    - **Conditions**: Non-normal data, ordinal data.

## 5. **Interpreting Results**

- **Rejecting the Null Hypothesis**: There is sufficient evidence to support the alternative hypothesis.
- **Failing to Reject the Null Hypothesis**: There is not enough evidence to support the alternative hypothesis; the null hypothesis stands.
