# Kickstarter Campaign Analysis

## Background

Over $2 billion has been raised using the massively successful crowdfunding service, Kickstarter, but not every project has found success. Of the more than 300,000 projects launched on Kickstarter, only a third have made it through the funding process with a positive outcome.

Getting funded on Kickstarter requires meeting or exceeding the project's initial goal, so many organizations spend months looking through past projects in an attempt to discover some trick for finding success. Excel Challenge: Organizie and analyze the database of 4,000 past projects in order to uncover any hidden trends.

---

## Process

Using the Excel table provided, modify and analyze the data of 4,000 past Kickstarter projects to uncover some market trends.

### Step 1:

- Use conditional formatting to fill each cell in the `state` column with a different color, depending on whether the associated campaign was successful, failed, or canceled, or is currently live.

  - Create a new column O called `Percent Funded` that uses a formula to uncover how much money a campaign made to reach its initial goal.

### Step 2:

- Use conditional formatting to fill each cell in the `Percent Funded` column using a three-color scale. The scale should start at 0 and be a dark shade of red, transitioning to green at 100, and blue at 200.

  - Create a new column P called `Average Donation` that uses a formula to uncover how much each backer for the project paid on average.

  - Create two new columns, one called `Category` at Q and another called `Sub-Category` at R, which use formulas to split the `Category and Sub-Category` column into two parts.

  - Create a new sheet with a pivot table that will analyze your initial worksheet to count how many campaigns were successful, failed, canceled, or are currently live per **category**.

  - Create a stacked column pivot chart that can be filtered by country based on the table you have created.

  - Create a new sheet with a pivot table that will analyze your initial sheet to count how many campaigns were successful, failed, or canceled, or are currently live per **sub-category**.

  - Create a stacked column pivot chart that can be filtered by country and parent-category based on the table you have created.

### Step 3:

- The dates stored within the `deadline` and `launched_at` columns use Unix timestamps. Fortunately for us, [there is a formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) that can be used to convert these timestamps to a normal date.

  - Create a new column named `Date Created Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within `launched_at` into Excel's date format.

  - Create a new column named `Date Ended Conversion` that will use [this formula](https://www.extendoffice.com/documents/excel/2473-excel-timestamp-to-date.html) to convert the data contained within `deadline` into Excel's date format.

  - Create a new sheet with a pivot table with a column of `state`, rows of `Date Created Conversion`, values based on the count of `state`, and filters based on `parent category` and `Years`.

  - Finally, create a pivot chart line graph that visualizes this new table.

---

## Research Questions & Analysis/Conclusions

1. Given the provided data, what are three conclusions we can draw about Kickstarter campaigns?

- First, based on the analysis, we can conclude that between year 2009 to 2017, out of 4064 Kickstarter campaigns around the world, there are 54% that were successful, 38% failed, and 9% canceled.

![ScreenShot1](/images/1.png)

- Secondly, based on the analysis, we can conclude that the categories that have the highest number of campaigns are, first, “theater”, which as 1369 campaigns, then second is “music” with 680 campaigns, and the third is “technology” with 600 cases. (Please see below image for reference.)

![ScreenShot1](/images/2.png)

    However, regarding the actual success rate among these categories, we can see that for “theater”, success rate is about 61.29%, whereas the “music” success rate is as high as 79.41%, and “technology” success rate is only about 34.83%. (Please see below image for reference.)

![ScreenShot1](/images/3.png)

    On the other hand, the category that has the fewest campaigns as well as lowest success rate is “journalism”, which only has 24 submissions and all 24 of them were cancelled.

- Thirdly, from the pivot-table based on the sub-categories, we can see that “plays” has the highest number of campaigns, 1066, which is about 25.91% out of the total of 4114 campaigns.
  (Please see below image for reference.)

![ScreenShot1](/images/4.png)

2. What are some limitations of this dataset?

   - There are some limitations of this dataset, for example, it would be better if we can obtain the links to each of the project to further analyze on how the actual content of the campaign and the presentation, such as graphic design and arrangement of the materials, etc., would affect the overall attractiveness and gain attention from the audience.

   - It would also be a good reference to know more about the team that creates this campaigns, for example, how many people are on the team, as well as the overall background and scale of the company. For example, some campaigns are created by one person only, but some are backed by an investment company, etc. With this information, we can further analyze regarding the relationship between the person/company that is operating the campaign, their resources, and the success rate.

3. What are some other possible tables and/or graphs that we could create?

   - There are several other possible tables/graphs that we could create, such as the pivot tables that show the relative successful and failed campaign percentage (%) in comparison to the overall number of campaigns, as created and shown in #2.
   - We could also create a table/graph to compare the categories against the overall time it took to complete a successful campaign.
   - Another table/graph we could create is to compare the successful and failed categories among different countries. This way, it can help people who want to start a campaign, to gauge further on the target market/country that they want to invest in.
   - Also, as mentioned in #2, if we can acquire more information regarding the company scale behind each campaign, we can create a table/graph based on the company size V.S. success rate, to further evaluate if the company resources have any impact on the success of the campaign. In addition, we can also create a table/graph to evaluate the relationship between the marketing/advertising resources that the companies invested in outside of the Kickstarter platform V.S. the time that the Kickstarter campaign took to be successful, to see if there’s any pattern between the two.

---

## Thank you!
