# Marketing-AB-Testing
Project on AB testing marketing campaigns to find the best campaign for the company to get more customers.
Dataset found on: https://www.kaggle.com/datasets/amirmotefaker/ab-testing-dataset/data

PACE Framework (Plan - Analyze - Construct - Execute)

Planning
To identify the strongest performing marketing campaign, this notebook will evaluate the campaigns through common marketing objectives:

ROAS: Identify which campaign is more cost-effective in generating conversions, and returns a higher return on advertisement spend (ROAS).
Reach: Identify which campaign achieved a higher number of impressions
Engagement: Identify campaign with more activity within the clicked webpage.

Analyze
Further investigation into correlation between variables in Control and Test Marketing Campaigns must be conducted to validate assumptions.

Construct
A polynomial regression model will be constructed to predict the number of Impressions, Website Clicks and Purchases. This will be used to identify optimum levels of expenditure on Control and Test campaign.

A polynomial regression model extends the concept of linear regression by allowing for non-linear relationships between the predictors and the target variable.

Execute
