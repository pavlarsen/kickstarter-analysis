# Kickstarting with Excel

## Overview of Project:

### This project has the intention to prove whether a successful campaign in Kickstarter will depend on the date it was launched or if the amount of money needed could be a factor determining if a campaign is too big to be funded.

---

## Analysis and Challenges

### Analysis of Outcomes Based on Launch Date

For this analysis, I had to group all the data relevant for the parent category "Theater" from the database that Laurie provided. Some key elements to identify if "date" is relevant for success were Date Created Conversion, Outcomes. With these elements, I could create a Pivot Table to group and count "successful", "failed", "canceled" campaigns. Then in order to visualize which months seem to be better to launch a campaign, I created a line chart.


![Captura de Pantalla 2022-09-25 a la(s) 11 42 53](https://user-images.githubusercontent.com/113866707/192155064-0c056251-167d-491f-88b9-a75dd99cd999.png)


![Theater_Outcomes_vs_Launch](https://user-images.githubusercontent.com/113866707/192155101-cd58a6bf-6db0-46a8-9bd1-6342207b5764.png)


### Analysis of Outcomes Based on Goals

For this analysis, the idea was to determine if certain levels of "Goal" for the campaign would impact on the possible outcome this for specific "Plays" subcategory. For example: "Is a $10,000 goal campaign too much for people to fund it?" For this analysis, in order to identify the percentage of success, failed and canceled campaigns, it was important to set certain levels for the Goal of the campaign. Between goals of $1,000 and $5,000 the brackets were formed of levels of $5,000. We also set brackets for goals below $1,000 and above $50,000. Whit this information, it was possible to notice that almost 85% of the Plays campaigns were set below $10,000. Then for these campaigns, below a goal of $5,000, between 73% and 76% of the campaigns succeed. A campaign with a goal beyond $50,000 is more likely to fail.

![Captura de Pantalla 2022-09-25 a la(s) 11 44 41](https://user-images.githubusercontent.com/113866707/192155150-3bec5a11-ad33-42d8-a4bb-703ff25afd24.png)

![Outcomes_vs_Goals](https://user-images.githubusercontent.com/113866707/192155155-4151d169-bc9c-4473-ae80-51fb40c8735d.png)


### Challenges and Difficulties Encountered

Some of the challenges that I faced was first to determine that the date on variable "launched at" was a date. Once it was figured it out that it was indeed in Unix timestamp, I converted it to normal dates. The next challenge I face was with the "countifs" formula was providing the accurate filtered data from the dataset. I verified the filters and checked all the data matched.

---

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

1.- Successful campaigns are launched between May and June, then it seems to be a downward trend afterwards. It is also the period where more campaigns for Theater are launched overall. Laurie will benefit from launching her Play campaign within May and June; however, she will face more competition from other Kickstarter looking for funding.

2.- I will recommend Laurie to avoid placing her campaign in the months of October, December and January since these months, seem to be the ones with more failures or cancelations.

- What can you conclude about the Outcomes based on Goals?

1.- If Laurie wants to have success in funding her play, she better place a goal of less than $15,000. It would be better for her to place goals of less than $5,000.

2.- Avoid campaigns with goals between $15,000 and $35,000 and beyond $50,000 since these tend to failure.

- What are some limitations of this dataset?

This dataset lacks to provide information on what makes a campaign successful or failure. Was there any other variable that made each of these campaigns’ better options for backers? where there more diffusion of the campaigns or communication? Was the "blurb" more appealing for the backers?  

- What are some other possible tables and/or graphs that we could create?

With the dataset provided, we could analyze trends within years of successful campaigns. Tables with more successful campaigns and try to derive what made them successful or failure. We could also need to look if there are any outliers within the data and determine if they should be kept, normalize or erase.
