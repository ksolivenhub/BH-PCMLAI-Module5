# BH-PCMLAI-Module5
This repository contains the practical application assignment for Module 5.
Additional details are provided in this activity's Juniper Notebook.

Notebook link: https://github.com/ksolivenhub/BH-PCMLAI-Module5/blob/de536bc25e102c975dfbb53ca70b43e1b0e814d1/prompt-ksoliven-fin.ipynb


## Guided Investigation Results:

### Conclusion

- There is a higher percentage of people not accepting Bar Coupon. 
    - `Delta is at 17.62%`
- The acceptance rate of people going less than 3 times monthly is more likely than more than 3 times monthly
    - `Acceptance rate at ~81%`
- Compared to all others who accepted the Bar Coupon, those who go to Bar once (1) monthly and over the age of 25 have a significant presence in the data set
    - `Acceptance rate at ~28%`
- The acceptance rate of people who went to the Bar once (monthly) and does not have a passenger kid has a significant presence in the data set
    - `Acceptance rate at ~48%`
    - `For this data sample, it is not affected by Age or Marital Status as the values are equal`
- An observation made is that Bar > 3 does not contain most of the data sample entries

***Based on this sampled data, Drivers who accepted the coupons could be hypothesized as follows:***
1. Bar < 3 contains most of data sample entries
2. Most drivers that go to the bar less than thrice (3) monthly is more likely to accept/use the coupon
3. Drivers are more likely to accept/use coupon if they have a Kid as a passenger


## Independent Investigation Results:

### Questions to explore

**Core question: What are the best performing coupon groups?**

1. Are the coupon expiration dates effective?
2. What is the best time/season to release the coupons for marketing?
3. Who to send the coupons?
    - This is based on the following factors:
        - Income
        - Marital Status
        - Has Children
        - Education
        - Gender
        - Age

### Findings/Conclusion

***Based on the sampled data and the overall results of this analysis from Q1 to Q3, the following assertions can be made:**
1. The Coupon types that have the best performance (based on analyzed features) are the following:
    - `Restaurant(<20)`
    - `Coffee House`
    - `Carry out & Take away`
2. The `higher the Coupon validity duration`, the higher chance that consumers will accept the coupon
    - A likely scenario is if the expiry is too long, the acceptance rate will decrease
        - The condition above most likely have an ideal threshold/range to maintain a positive acceptance rate
        - There is not enough data to predict this parameter
3. The data set provided for this activity contains useful information to predict consumer behaviour in a `Sunny` weather
    - There is a positive correlation between temperature and coupon acceptance
4. For the best performing Coupon groups, it is ideal to offer them between `10 AM to 6 PM` as a high coupon acceptance were observed
5. `Cheap Restaurants and Coffee House` have similar characteristics relative to time and temperature on a Sunny day
    - Visits are more frequent before noon (7AM to 10PM) on a warm temperature
    - After 6 PM, visits for these parameters are also seen during the cold temperature range
6. `Carry out & Take way` is not dependent on temperature
7. To maximize potential profit, any marketing campaign related to these best perfoming coupons should primarily target the following consumers:
    - Age between `21-31` and `50+`
    - Marital Status of `Single, Unmarried, and Married Partners`
    - `No Children`
        - It would be interesting to explore/confirm if this parameter's acceptance rate is indeed higher when driving with Kids
    - Income is below `$62,500` and above `$100,000`

### Recommendation

1. Consider that the following types of establishments will generate the most coupon acceptance rate and leverage this knowledge to the owner's advantage
    - `Restaurant(<20)`
    - `Coffee House`
    - `Carry out & Take away`
2. Use the **predicted parameters** above to improve success rates of Coupon marketing campaigns
3. Gather more data related to coupon acceptance in other weather/time conditions to create a full view of which businesses are running successful campaigns.
4. Explore the Trip Attributes in relation with Coupon and User Attributes as this was not incorporated on this analysis.
