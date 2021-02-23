# Kickstarter-Analysis

## Overview Of Project
In order to best position Fever for a successful Kickstarter campaign, a data analysis was performed on a dataset of Kickstarter data (linked below). This particular analysis looks at two major measurements: Theater Outcomes By Launch Date, and Outcomes Based On Goals. These two were chosen as a means to determine the best target goal amount and best launch date to increase the probability of success for funding of Fever. 

## Analysis and Challenges

### Outcomes By Launch Date

#### Explanation
The Theater Outcomes By Launch Date sheet measures outcomes based on the month of the year in which a kickstarter campaign is launched. Cultural and financial cycles throughout the year will influence when people will be most likely to invest money into financing a kickstarter project, so it makes sense to assess the timeframes where campaigns appear to be most successful. While the image below does not specify plays as compared other theatrical campaigns or take into consideration variations by year, there does not seem to be any major difference in the pattern visualized here when analyzed for these potential shifts in pattern. 

#### Methodology
This information was calculated by creating a pivot table to explore the outcomes of campaigns in the Theater category based on groupings of months of the year with the option to choose the year(s). This measurement did not originally allow for differentiation by country or subcategory, however these variables were added to expand upon understanding of outcomes. It appears that the patterns hold true across these other factors of analysis.  

#### Visuals
![Theater Outcomes By Launch Date](https://github.com/ghynox/Kickstarter-Analysis/blob/main/Outcomes%20Based%20On%20Launch%20Date.png)

###Outcomes Based On Goal

#### Explanation 
The Outcomes Based On Goal sheet is designed to explore outcomes based on the amount of money requested for the target goal of campaigns in the Play subcategory. Many psychological factors influence when and how people will invest money in Kickstarter campaigns. One of these factors is the overall goal amount of a project. When measuring this data, we were able to see a clear pattern indicating that there are ideal value ranges to increase the probability of success. 

#### Methodology
To measure the outcomes based on target goals for campaigns, a table was created that broke down goal amounts into ranges below $1,000 and then by $5,000 increments with the final row being greater than $50,000. Values for each of the outcome variables were calculated using a COUNTIFS formula which specified the desired outcome, subcategory as Play, and the appropriate range for the goal amounts. These numbers were then SUMmed to gather our totals and then percentages were calculated. This table and the associated graph do not allow for more in-depth study based on other parameters such as timeframes or countries, however it does include more than 1000 campaigns and shows some notable differences in rates of success and failure. 

#### Visuals
![Outcomes Based On Goal](https://github.com/ghynox/Kickstarter-Analysis/blob/main/Outcomes_vs_Goals.png)

### Challenges
This assessment provided a number of challenges including having to backtrack to confirm formula outcomes that appeared to be incorrect at first glance and having to trouble shoot errors in formulae coding that gave incorrect data outputs. The first was found when writing the COUNTIFS formula to determine the number of Plays were canceled. The formula produced 0’s across the board and at first this appeared to be an error in the formula. Upon checking in the Kickstarter sheet using filters, it was determined that there were in fact no plays that were canceled. The second noted challenge occurred when calculating the Outcomes Based On Goals sheet as well, where the 40,000-44,999 range had an typo that produced a much larger range ending at 54,999 and producing incorrect data. This was corrected after being compared to the correct graph from the instructions, but the experience definitely reinforced the idea of slowly and methodically reviewing code and formulae to make sure no errors are present. 

## Results

### Best Month For Launch (Outcomes Based On Launch Date) 
1. Best Month For Launch: May
2. Worst Month For Launch: December
Given this data, it is plain to see that Play campaigns launched in May tend to provide the greatest probability for success with June and July following in that order with 67%, 65%, and 63% chances for success respectively. It is also quite clear that December appears to be the absolute worst month in which to launch a campaign for a play as successes and failures are nearly a 50/50 split. 

### Best Goal Range (Outcomes Based On Goals)
1. $0-$5000
2. $35,000-$45,000
Based on the data provided, and as visualized in the image below, we can see that there are two ranges that have a higher probability for success and two ranges that have a higher probability for failure. Campaigns under $1000 showed the highest success rate at 76% and between $1000-$5000 was 73%. Campaigns between $35,000-$45,000 showed 67% chance of success. Given that Fever will likely require more than $1000 to operate, this may not be the ideal range for the target goal. Once the projected budget for Fever is completed, it will be possible to determine which of these ranges provides the best target range to increase success probability.

### Limitations Of Dataset
This particular dataset does have a few limitations that will reduce the overall accuracy of projections made. 
1. The data stops in early-mid 2017. This data does not include the most current data and will miss any new trends that may be occurring based on recent global and regional economics or cultural preferences.
2. The initial parameters for assessment did not allow for as detailed of an exploration as should be performed for an accurate measure of how Fever will perform in different markets, and in some cases even observing the specific of a Play versus other theatrical campaigns. 
3. Assessment using this dataset also does not take into accout the type of play or synopsis. We do not have information regarding how plays of this type are received by the global population or by the country populations. 

### Potential Additional Tables/Graphs:
1. Breakdowns of Outcomes Based On Goals including country markets.
2. Outcomes Breakdown sheet showing what categories and subcategories achieved which outcomes to get a view of how Plays compare to other subcategories of Theater and how Theater compares to other categories (Sheet Added)
