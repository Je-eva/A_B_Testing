In this project, I performed A/B testing to evaluate the effectiveness of a change (like a new feature or design) in improving click-through rates. The dataset consists of two groups: an experimental group (exposed to the change) and a control group (which did not receive the change). I started by loading and exploring the data using basic descriptive statistics to understand the distribution of clicks across both groups.

I used **seaborn** for visualizing the click distribution between the experimental and control groups. The countplot helped in illustrating how the number of clicks was distributed across the two groups, with a custom color palette distinguishing between "click" (1) and "no-click" (0) outcomes. I also annotated the bars with the percentage of clicks in each group to provide a clearer comparison.

Next, I focused on calculating key metrics such as the proportion of clicks in each group, the **pooled click probability** (which assumes that both groups come from the same population under the null hypothesis), and the **pooled variance**. The pooled variance accounts for the combined variability from both groups and helps estimate the spread of the proportions. Using these, I computed the **standard error (SE)** and the **Z-statistic** to test whether the difference in click rates between the experimental and control groups was statistically significant. 

To assess statistical significance, I compared the test statistic with the **critical value (Z_crit)** from the standard normal distribution and calculated the **p-value**. If the p-value was less than or equal to the significance level (alpha = 0.05), I rejected the null hypothesis, indicating that the difference observed was unlikely to be due to random chance and was, therefore, statistically significant.

In addition to statistical significance, I also performed a practical significance check using the **minimum detectable effect (MDE)**, which defines the smallest difference in click rates that would be considered meaningful. I compared this value against the 95% confidence interval of the observed difference. If the lower bound of the confidence interval was greater than or equal to the MDE, it confirmed that the observed difference was not only statistically significant but also practically meaningful.

Overall, the combination of these statistical tests allowed me to assess both the significance and the impact of the changes made in the experimental group, helping to draw actionable conclusions about whether the experimental design had a real effect. This methodology is essential for making data-driven decisions, ensuring that any changes made are both statistically and practically beneficial.


![image](https://github.com/user-attachments/assets/27bd0d4f-9f78-43fc-9c7f-05decb44f1f9)
As you can see from the image, the control and the experimental are the two different use case scenarios for the application and its been found out that, the experimental one is found to be more business efficient , providing with more CTR

<h2>Thanks to FreeCodeCamp and LunarTech for this course</h2>


