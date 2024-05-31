# Marketing-AB-Testing
Full Notebook Link: https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/blob/main/%5BFINAL%20ANALYSIS%5D%20AB_Testing.ipynb

Project on AB testing marketing campaigns to find the best campaign for the company to get more customers.

Data Analysis Techniques used: Correlation Heatmap, Polynomial Regression, Visualization of Relationships (Pie Chart / Scatterplot), Trend Lines, Time Series Anaylsis

Dataset found on: https://www.kaggle.com/datasets/amirmotefaker/ab-testing-dataset/data

**Actionable Business Recommendations**

1. The number of add to carts is high for the control campaign, but the conversion rate is low. The client should consider launching follow-up campaigns to target the audience that has added the product to cart, resulting in higher sales.
2. Run both marketing campaigns simultaneously to achieve higher sales, at the spend points highlighted in the table below. Moreover, run them for longer periods of time (3-4 months, rather than 1 month) to receive more accurate datapoints and allow the algorithm to optimise itself.

**Exploratory Data Analysis**

<div align="center">
<img width="389" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/6809aeea-5744-4298-9a39-fd64bf308f79">
<img width="400" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/b343bde6-a958-4e70-a9fc-0860ed7db6b6">
</div>

For control campaigns, there appears to be a stronger correlation between USD Spend and Impressions (0.26) / Reach (0.19). Thus the control campaign may be a good method for the client to reach larger audiences and increase their awareness by increasing their spend on the campaign. However, the negative correlation between impessions, website clicks and viewed content, suggest that the target audience may not be entirely relevant, as the number of impressions rise, the number of website clicks and viewed content falls.

The test campaign differs from the control campaign in that the amount of spend does not necessarily correlate to higher impressions and reach, but rather to more of the audience adding to cart (15%). This suggests the campaign is more focused, this is supported by the correlation between add to cart and purchases of 80%, suggesting a higher conversion rate. Moreover, the moderately strong correlation between viewed content, website clicks, add to cart, and purchases suggest that the advertisement generally matches what users are searching for.

**Identifying Trends in Variables: Scatter Plots**

<div align="center">
<img width="333" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/45a0ad23-0114-4e02-af44-d0f3e0feaec6">
<img width="329" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/3d0e60c9-ba5f-4163-b83e-9e5ac7f9042b">
</div>

The higher conversion rate from added to cart and purchases is evident in the test campaign when plotted on the scattterplot. However, it is worth noting that the control campaign has resulted in more users adding to cart, but not finishing the purchase, therefore it is recommended to increase the number of follow-up advertisements for the control campaign.

Meanwhile, when comparing the total spend and impressions of each campaign, it can be seen that the assumption of a broader campaign for Control is seen, reaching a higher number of impressions (~40,000 more) than the Test Campaign.

<div align="center">
<img width="329" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/90c3a06d-8d00-479b-aad6-706eb902a7f9">
<img width="332" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/575824fe-7396-4245-b05c-491d0684c6cb">
</div>

However, as the number of impressions increases, Control campaigns exceeding 120,000 impressions begin receiving a lower engagement than the test campaign, receiving fewer views and suggesting a deterioration in audience quality, whilst the test campaign continuously engages relevant audiences due to its narrower specifications.

When considering overall spend and purchases however, there is no clear trend, suggesting that whilst the control campaign captures a broader market and results in a lower conversion rate, due to its higher number of impressions and add to carts, the outcome of total purchases is similar to the test campaign. Therefore, there is not a strong need to remove one campaign but rather keep both.

**Polynomial Regression: Optimal Spend calculated according to different marketing objectives**

Optimal spend was calculated according to maximum impressions, purchases,and ROAS. Below is an example of optimal spend for maximum purchases.

<div align="center">
<img width="348" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/2d42e7c8-6d6b-4163-9467-d6e88856c24e">
<img width="349" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/8e2514d9-3639-42f8-a476-1f8f3e5e5b6d">
</div>

Ultimately, the optimal spend is calculated and summarized below:
<div align="center">
<img width="555" alt="image" src="https://github.com/keithchhh/Marketing-AB-Testing--Polynomial-Regression/assets/145700071/ee59b4dc-0101-43e9-9a0b-3f58c2bd10c2">
</div>

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
