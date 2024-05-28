# Marketing-AB-Testing
Project on AB testing marketing campaigns to find the best campaign for the company to get more customers.

Data Analysis Techniques used: Correlation Heatmap, Polynomial Regression, Visualization of Relationships (Pie Chart / Scatterplot), Trend Lines, Time Series Anaylsis
Dataset found on: https://www.kaggle.com/datasets/amirmotefaker/ab-testing-dataset/data

**PACE Framework (Plan - Analyze - Construct - Execute)**

**Planning**
To identify the strongest performing marketing campaign, this notebook will evaluate the campaigns through common marketing objectives:

1. ROAS: Identify which campaign is more cost-effective in generating conversions, and returns a higher return on advertisement spend (ROAS).
2. Reach: Identify which campaign achieved a higher number of impressions
3. Engagement: Identify campaign with more activity within the clicked webpage.

**Analyze**
Further investigation into correlation between variables in Control and Test Marketing Campaigns must be conducted to validate assumptions.

**Construct**
A polynomial regression model will be constructed to predict the number of Impressions, Website Clicks and Purchases. This will be used to identify optimum levels of expenditure on Control and Test campaign.

A polynomial regression model extends the concept of linear regression by allowing for non-linear relationships between the predictors and the target variable.

**Execute**
Actionable Business Recommendations
1. The number of add to carts is high for the control campaign, but the conversion rate is low. The client should consider launching follow-up campaigns to target the audience that has added the product to cart, resulting in higher sales.
2. Run both marketing campaigns simultaneously to achieve higher sales, at the spend points highlighted in the table below. Moreover, run them for longer periods of time (3-4 months, rather than 1 month) to receive more accurate datapoints and allow the algorithm to optimise itself.
