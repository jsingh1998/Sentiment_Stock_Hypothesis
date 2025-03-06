In this project, I analyzed the relationship between social media sentiment and stock market performance using 4.3 million tweets from 2015 to 2020 for major companies: Apple, Google, Amazon, Microsoft, and Tesla. By leveraging VADER and BERT sentiment models, I explored whether sentiment scores could predict stock growth or decline on a daily basis.

1. Data Preparation: Merged daily stock performance data with previous day's sentiment scores and categorized days as either "growth" (positive stock return) or "decline" (negative stock return).

2. Initial Findings (VADER): VADER sentiment scores satisfies assumptions for parametric test. No significant difference in sentiment scores between growth and decline days when using VADER sentiment analysis and independent samples t test (p-value > 0.05 from t-test).

3. Normality Check (BERT): Found that BERT sentiment scores were not normally distributed for either growth or decline days, leading to the use of the non-parametric Mann-Whitney U test.

4. Key Result (BERT): Mann-Whitney U test revealed a statistically significant difference in BERT sentiment scores between growth and decline days (U-Statistic: 9911476.0, p-value: 4.65e-06).

Conclusion: While VADER showed no significant difference, BERT sentiment scores revealed a meaningful difference between growth and decline days, suggesting that sentiment measured by BERT may be a useful factor in understanding stock performance. This also suggests that context-aware sentiment analysis (BERT) can better capture the relationship between social media sentiment and stock market behavior.
