# Prosper Loan Data
Prosper was founded in 2005 as the first peer-to-peer lending marketplace in the United States.
Since then, Prosper has facilitated more than $17 billion in loans to more than 1,010,000 people.

## Dataset

This data set contains 113,937 loans with 81 variables on each
loan. The data set can be found [here](https://s3.amazonaws.com/udacity-hosted-downloads/ud651/prosperLoanData.csv) for download. There is a  data dictionary which explains the variables in the data set which and
can be found [here](https://docs.google.com/spreadsheets/d/1gDyi_L4UvIrLTEC6Wri5nbaMmkGmLQBk-Yx3z0XDEtI/edit#gid=0).



## Summary of Findings

In the exploration I asked the "What factors affect the outcome of Lenders Yield?". These are my findings:

1. The lower the Prosper Score the higher the Lenders Yield and the higher the Prosper score the lower the yield. Riskier loans have higher lender yields. By exploring a little further I found that those with higher prosper scores are given lower interest rates. There is only a slight glitch between 5 and 4 then continues dropping until prosper score 10. There are outliers on both sides of the scores.
2. The scatter plot shows a strong positive relationship where lender yield increases with borrower rate increase. As the borrower rate increased, the Lender yield increased
3. There is a good positive relationship between estimated return and lender yield. The lender yield increases as the estimated return increases.
4. The Lender yield decreases as the income range increases and vice versa
5. Most loan values are concentrated below 15k. The higher loans also have a lower yield than the smaller loans
6. From the line chart the Lenders Yield is always higher than the estimated return for all the years plotted


Adding other variables to the prosper score and lender yield I found the following:

1. Prosper score between 7 to 10, the best average yields are for those loans that are 60 months long. For prosper scores 2, 3, 5 and 6, loans with 36 months tenure have better yields. Its only Prosper score 4 that has the best yield on 12 month loans. Overall the 12 month term loans have the worst yield in majority of prosper scores.
2. For every prosper score the average Lender yield is lower for homeowners. The only exception is the prosper score 1 where the homeowner loan has a marginally higher average yield than the borrower without a home.
3. The prosper score of 2 to 7, lenders yield is higher when the borrower is in a group. This is however different for all other prosper scores where those not in a group offer better yields for the lender.
4. In Listing Category, Cosmetic procedures have highest Lender yield and the lowest is boat


## Key Insights for Presentation

For the presentation the focus will be on the factors that affect Lenders yield. The distribution of the Lenders yield will be introduced followed by the box plot of the Lenders yield and Prosper score. Then I used a Scatter plot to examine the relationship between Lender yield and Borrower rate. Next I used a Heat map to plot the relationship bewtween Lender yield and original amount borrowed.
I found the relationship between the Lender yield and Prosper score interesting so I decided to focus on them and add other variables to gain deeper insights. This was  then be followed adding the interaction with other variables like the borrower rate, home ownership and loan terms. The variables Loan term, Homeownership and loans terms were systematically added to the box plots.
For the loan term I wanted to see what yields they offer and how they are distributed within the Prosper score. Color encodings were used to clearly distinguish between the different loan terms. The most significant insight here is that the 12 month term loans offer the least yield to Lenders. From Prosper score 2 to 6 the 36 month loan term offers best yields while for 7 to 10 the best yields are in 60 month loans. The higher Prosper score of 8 to 10 have alot of outliers on the upside which show there is a chance of getting higher yields. For the lower score 1 and 2 most of the outliers are on the lower side indicating possibility of getting lower yields.
Next I added home ownership to the Lender yield and Prosper score and found that for every prosper score the Lender yield is lower if the borrower is a  homeowner. The only exception is the prosper score 1 where the homeowner loan has a maginally higher average yield than the borrower without a home. Going further I added Borrowers in group and those not in a group. The prosper score of 2 to 7, lenders yield is higher when the borrower is in a group. This is however different for all other prosper scores where those not in a group offer better yields for the lender.
Finally I examined the interaction between the Lender yield and the Estimate given by Prosper loans before the investment is made. From the line chart I found that they followed the same pattern. The good news is that for all years available, the Lender yield has outperformed the Estimated yield for all years on record.


## Feedback Observations

1. The box plot and scatter plot do not have plot name in the title. Those with no knowledge of plots wont know what it is.
2. Add notes about the variables so that viewer can get an explanation without asking
3. There are too many slides, consider reducing the number of slides and compressing the main message so that it doesnt get lost in all the noise.

## Changes implemented from Feedback
1. I made sure all plots on the slide deck have plot kind written in Title
2. I added some notes to slides containing definition of variables
3. I reduced the number of slides and focused the message to what is there now


## References Used
www.stackoverflow.com
www.lindsaymoir.com
https://github.com/jeremymonger/communicate-data-findings/blob/master/Prosper_Loan_Exploratory_Notebook.ipynb
