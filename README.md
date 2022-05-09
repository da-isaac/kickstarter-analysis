# Kickstarting with Excel

## Overview of Project

### Purpose

The client, Louise, recently launched a campaign to raise funds for her play, Fever. She is wishing to compare the success of her own campaign to the campaigns of others, specifically those also seeking funding for theater/plays. She has asked that we find insights into what impact the launch dates and funding goals have on a campaign's success.

## Analysis and Challenges

### Challenges and Difficulties Encountered

The raw data used for the analysis was fairly clean, but some extra data manipulation and extraction was needed in order to use for analysis. This included generating the appropriate date from the UNIX timestamp, further splitting the category pairs, and other campaign metrics. Luckily, there were no major data holes or corrupted data, so all data receieved for this project was useable.

### Analysis of Outcomes Based on Launch Date

After converting the UNIX timestamps, the data was ready to be viewed through a temporal lens. While there were so many types of Kickstarter campaigns, the decision was made to filter down to only those related to "theater", since those would be the most related to Louise's project. Dates were then grouped by month (rather than year or day) through a pivot table to easily filter between desired data.

### Analysis of Outcomes Based on Goals

Due to the number of campaigns in the dataset, it would've been unrealistic to try analyzing the data on every campaign funding goal, as the variance between each individual amount would've been too large to find patterns in. Instead, the data was grouped into more general categories and then analyzed for any trends from there.

## Results

- What are two conclusions you can draw about the Outcomes based on Launch Date?

May is overwhelmingly the month with the most success, suggesting it is one of the better times to launch a campaign. Perhaps this is caused by the time and freedom that accompany the summer months. 
Alternatively, while not many campaigns were canceled, it seemed to be common for Kickstarters launched within January to cancel more frequently than those that didn't.

- What can you conclude about the Outcomes based on Goals?

It appears that most campaigns do better if they fall under $5000. While campaigns in the ranges of $35000 - $44999 seem to succeed as well, not many campaigns actually fall in this range.

- What are some limitations of this dataset?

Within the "Outcomes Based on Goal" data, it should be noted that the data distribution is skewed right, meaning the majority of campaign goals were set at less than $30,000. This explains the somewhat sporadic lines to the right of the graph and why they seem to deviate significantly from the stable lines on the left. A way around this would be to wait for more Kickstarter campaigns for plays, but there is no way of knowing how long it would take to achieve a more significant sample size.
Another element that is missing entirely from the dataset is information about rewards backers get for supporting the campaign. It is farily common for campaign owners to provide incentives for providing financial support, and this could be one of the things that pushes helps determine successful campaigns from unsuccessful ones. Perhaps it also explains why some campaigns are so much more successful than their original goal.

- What are some other possible tables and/or graphs that we could create?

Two big areas that were not investigated at all were the staff_pick and spotlight columns. It is reasonable to assume that spotlighted campaigns have a higher chance of being successful than those that are not, and the same may be true for those that were staff picked. Another area that may reveal trends is the average funded by doner. Perhaps campaigns succeeded because the doners themselves were more financially privileged than the doners in campaigns that failed.