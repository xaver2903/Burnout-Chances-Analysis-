# Burnout-Chances-Analysis
Remote Work & Employee Burnout Analysis
📌 Project Overview

This project analyzes remote work behavior data to identify factors associated with employee burnout. Using statistical analysis and linear regression modeling, the goal was to determine whether remote work characteristics such as work hours, sleep, meetings, and task completion influence burnout levels.

The dataset contains 1,800 daily employee records with 11 variables measuring workload, productivity, and burnout risk. The analysis focuses on identifying the strongest predictors of burnout and translating findings into actionable business recommendations.

🎯 Business Question

Does working from home impact employee burnout rates?

More specifically:

Which work-related factors are most associated with burnout?

Are time-based measures (work hours, sleep) or performance-based measures (task completion) more important?

How well can we predict burnout using regression modeling?

📊 Dataset

Source: Kaggle – Work From Home Burnout Dataset

Observations: 1,800 daily records

Variables: 11 total

9 Numeric (work_hours, sleep_hours, meetings_count, task_completion_rate, burnout_score, etc.)

2 Categorical (day_type, burnout_risk)

Each row represents one employee’s daily work activity.

🔎 Exploratory Data Analysis
Data Cleaning

Verified data types using df.info()

Confirmed no missing values

Confirmed no duplicate records

Ensured numeric variables were properly formatted for modeling

Statistical Insights

Average burnout score: 44.01

Average work hours: 6.52 hours/day

Average sleep: 7.00 hours/night

Average task completion rate: 72.31%

Burnout showed significant variability across employees, while sleep and work hours were more tightly distributed.

📈 Modeling Approach
Simple Linear Regression

Burnout score regressed on work hours

Statistically significant but very weak explanatory power (R² = 0.014)

Multiple Linear Regression

Included workload, performance, and sleep-related predictors

Strong overall model fit (Adjusted R² = 0.922)

Final Model

After backward elimination and multicollinearity checks, the best-fit model included:

Burnout Score = 154.99 − 1.53(Task Completion Rate) − 0.71(After-Hours Work)

Key findings:

Task completion rate is the dominant predictor of burnout

Higher task completion is associated with significantly lower burnout

Time-based measures (work hours, sleep) were not strong predictors once performance was included

💡 Key Insights

Burnout is more strongly linked to performance efficiency than total hours worked.

Simply working longer hours does not necessarily increase burnout.

Improving task clarity and completion efficiency may be more effective than reducing hours.

🛠 Tools Used

Python

pandas

matplotlib

seaborn

scikit-learn

Jupyter Notebook

⚠️ Limitations

This dataset focuses only on workplace-related variables and does not include external factors such as personal stress, family obligations, or health conditions. Therefore, results should be interpreted from an employer-focused perspective only.

🚀 Business Recommendations

Organizations should:

Focus on improving task efficiency rather than extending work hours

Reduce unnecessary interruptions

Monitor after-hours work to ensure flexibility, not overload

Provide tools that improve productivity and clarity

Improving task completion efficiency appears to be the most effective strategy for reducing employee burnout.
