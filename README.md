#  Team 22, Duke Datathon 2018


🥇1st Place Team
📈 Big Data Energy

## Background
[Duke Datathon](http://dukeml.org/datathon/) participants have a 8-hour time limit to analyze a given data prompt in any
creative and insightful way. The 2018 Dataset is provided by [Credit Sesame](https://www.creditsesame.com/), a credit-reporting website. Participants were given the following 3 datasets:
- **A. User Profile**
  - Description: Snapshot of the user’s demographic and credit profile information at the time of signup.
  - Size: 285,619 rows, 38 columns, 1 row per user
- **B. First Session**
  - Description: detailed user action logs of each user’s first session on the site. A session is defined as an unbroken series of actions on the site (typically referred to as “clickstream”). One-to-many relationship between the user profile and this dataset defined by user ID.
  - Size: 8,755,480 rows, 16 columns, average 30.75 rows per user
- **C. 30-day User Engagment**
  - Description: summaries of the actions taken during each user session that occurred within the user’s first 30 days. A session is defined as the time period on the site between login and explicit logout or automated timeout. This should be a fairly sparse dataset for the different types of events. There is a one-to-many relationship between the user profile and this dataset defined by user ID.
  - Size: 1,179,988 rows, 40 columns, average 4.14 rows per user

## Proposition
Credit Sesame, a service that offers free credit score and credit report analyses, employs a business model that is sustained by revenue generated from targeted advertisements to consumers. Credit Sesame profits when users choose to consult these external offers by clicking ‘apply’ on a Credit Sesame recommendation page. 

**Our team sought to analyze the most important factors that drive consumers to click ‘apply’ and therefore become what we henceforth label a ‘valuable customer’ in the eyes of Credit Sesame.**

## Solution
- **A. Random Forest Classification Model** - Our team presents a machine learning model which can accurately predict whether users will/will not convert into valuable customers 71% of the time. Our model is validated using a 3-Fold Cross Validation and tested on a 20% Hold-out Testing set. Our model performance is further evaluated using a Confusion Matrix and a ROC curve. Using our well-preforming machine learning model, we were able to identify metrics that are most impactful in user conversion.

- **B. Tableau Visualization Dashboard** - We also present a handy Tableau visualization dashboard which allows Credit Sesame to view these important factors as well as the distribution of customers across the country according to several categorical buckets. This is useful in quickly determining location-based demographic info of current users and could be used in the future to predict patterns in new ones.

## Components
- **A. Jupyter Notebook** 
  - Description: Code composing of data wrangling, model building and model evaluation process.
  - Files: Jupyter Notebook code in .ipynb & .pdf format
  - Location: `team22_jupyter` folder
- **B. Tableau Dashboard**
  - Description: Visual representation of key user conversion metrics.
  - Files: Tableau Dashboard in .twb & .pdf format
  - Location: `team22_tableau` folder
- **C. Report** 
  - Description: 5-page Written Report documenting procedures and outcomes, used for first-round judging.
  - Files: Written Report in .docx & .pdf format
  - Location: `team22_report` folder
- **D. Presentation**
  - Description: 8-slide Powerpoint summarizing procedures and outcomes, presented during final-round judging.
  - Files: Presentation in .ppt & .pdf format
  - Location: `team22_presentation` folder
