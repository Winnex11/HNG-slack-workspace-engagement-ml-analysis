# HNG Slack Workspace Engagement Analysis & Prediction

## Project Overview
This project analyzes activity data from the HNG 13 Slack workspace to understand engagement patterns, identify behavioral trends, and predict members at risk of low engagement. Using exploratory data analysis, feature engineering, and machine learning models, the project delivers actionable insights supported by an interactive Power BI dashboard.

The analysis covers the full internship period and demonstrates how data analytics and predictive modeling can be applied to manage and improve engagement in large online communities.

## Objectives
The main objectives of this project were to:
- Analyze Slack workspace activity and engagement trends
- Engineer meaningful behavioral features from raw activity data
- Build and evaluate machine learning models to predict low engagement
- Publish interactive dashboards for stakeholder decision-making

## Dataset Overview
The dataset captures Slack activity during the HNG 13 internship period (October 15 – December 6, 2025).

**Key dataset components include:**
- Member profile information (role, account type)
- Messaging activity across public channels, private channels, and DMs
- Daily active user logs
- Channel-level engagement statistics
- Product and stage performance data

**Dataset scale:**
- 13,000+ unique members
- 3,000,000+ messages
- 56 channels
- 53 days of activity
- 12 internship products

## Tools & Technologies
- Python (Pandas, NumPy, Scikit-learn)
- Jupyter Notebook
- Power BI
- Microsoft Excel

## Feature Engineering
To improve predictive accuracy, several engagement-based features were engineered, including:
- Total messages posted per user
- Number of active days
- Average messages per active day
- Public, private, and DM message ratios
- Consistency score based on posting behavior
- Engagement probability (model output)

These features capture both **activity volume** and **behavioral consistency**, which are critical indicators of engagement.

## Exploratory Data Analysis (EDA)
EDA focused on understanding:
- Daily message volume trends
- Daily active user patterns
- Channel usage and engagement distribution
- Member engagement by role, account type, and activity level
- Contribution imbalance between highly active and inactive members

Key findings showed strong early engagement, followed by a steady decline, with a small subset of users contributing the majority of activity.

## Machine Learning Modeling
Two classification models were developed and evaluated:
- **Logistic Regression** as a baseline, providing interpretability and linear insights
- **Random Forest Classifier** to capture non-linear behavioral patterns and feature interactions

Model performance was evaluated using AUC, and Random Forest outperformed Logistic Regression. The final model outputs include:
- Engagement class (High / Low)
- Engagement probability score
- Risk category (High, Medium, Low)

These predictions were exported for dashboard visualization.

## Dashboard Insights
The Power BI dashboard consists of five main sections:
- **Daily Activity & Trends:** Message volume and active user trends across the internship timeline
- **Member Engagement Analysis:** Distribution of engagement levels and user behavior patterns
- **Channel Performance Analysis:** Channel usage, engagement rates, and efficiency
- **Product Excellence Dashboard:** Performance of internship products across stages
- **Prediction Analysis:** Visualization of engagement risk, probability scores, and behavioral drivers

The dashboard enables stakeholders to quickly identify engagement challenges and intervene proactively.

## Business Value
This project demonstrates how analytics and machine learning can:
- Detect early signs of disengagement
- Improve community and program management
- Optimize communication strategies
- Support data-driven decision-making in large digital platforms

## Limitations
- Analysis is based on a fixed internship time window
- User deactivation impacts engagement trends
- Some profile attributes were missing or unspecified

## Conclusion
The analysis reveals that engagement in large online communities is highly uneven and declines over time without intervention. By combining feature engineering, predictive modeling, and interactive dashboards, this project provides a scalable framework for monitoring engagement and identifying at-risk users before disengagement becomes permanent.

## Files in This Repository
- `hng_slack_analysis_ml.ipynb` – Full Python analysis, feature engineering, and modeling
- `report/hng_slack_workspace_report.pdf` – Detailed analytical and modeling report
- https://app.powerbi.com/view?r=eyJrIjoiOTFkZWQ3YTItZTdiYi00NGM0LWE2NTYtNzlkYWJiOGQ4YWU0IiwidCI6IjM5MTM5MTFjLWQ3NjUtNDg2Ny04Zjk5LTI3MzRlMWIyMDhlZSJ9 – Interactive Power BI dashboard documentation
