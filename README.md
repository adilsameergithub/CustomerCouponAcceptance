# CustomerCouponAcceptance
Analysis and Investigation of coupon dataset to see if Drivers/Customers Accept the Coupon

**Notebook**: [CustomerAcceptanceOfCouponsInvestigation.ipynb](CustomerAcceptanceOfCouponsInvestigation.ipynb)

**Data Set**: [coupons.csv](coupons.csv)

**Problem**: will the Customer Accept the Coupon?

The data set used in this notebook assignment was provided. The data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50). 

The overall quality of the data set was generally good and didn’t need much cleaning or transformation.
The # of duplicate rows were a very small portion and hence were not removed. 
The null value columns within the dataset were relatively small as well and were kept as is as they shouldn’t have impacted any of the analysis or plots.

Below is a visualization of the distribution of the various coupons accepted with “Coffee House” being the most popular,

<img width="589" height="565" alt="Screen Shot 2026-03-21 at 10 28 03 PM" src="https://github.com/user-attachments/assets/beaca0b5-d049-4471-a968-be626cac0065" />




**Findings**:

The major focus was to analyze and investigate the “Bar” coupon acceptance data. See below a few highlights based on the data analysis,
* 81% of the drivers that accepted the coupon went 3 or fewer times to a bar a month.
* Drivers that tend to have the highest rate of acceptance were around age 26 and who go to bars more than once a month, but it starts reducing as you get older. In addition, it starts peaking again after age 35. Under the age of 25, the rate of acceptance is at the lowest levels.

Additional analysis was done on the data exploring the Coffee House coupon, see below few observations,
* This was the largest and most popular coupon accepted.
* The coffee House coupon has almost a 50/50 split acceptance & rejection ratio.
* Singles & Married Partners tend to accept coupons for Coffee houses at a higher ratio.
* From an age grouping perspective, 26 & younger tend to accept coupons for Coffee Houses at a higher ratio.

Please see associated notebook for additional analysis and visualizations.

**Next Steps and Recommendations**: Based on the above analysis, other coupon categories should be investigated as well to complete the analysis and based on the results, the coupons can be served or advertised more towards those groups that have a higher acceptance ratio.
