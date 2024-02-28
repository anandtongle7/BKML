This directory contains project which aims at determining if the customer will select coupon offered or not using data analysis & visualization 

The directory contains following info: 

(1) Data : A csv formatted data is taken from UCI machine learning repository and was collected via a survey on Amazon Mechanical Turk. 
The survey describes different driving scenarios, including the destination, current time, weather, passenger, etc., and then asks people 
whether they will accept the coupon if they are the driver. Answers given that the users will drive there "right away" or "later before the coupon expires" 
are labeled as "Y = 1", and answers "no, I do not want the coupon" are labeled as "Y = 0". There are five different types of coupons—less 
expensive restaurants (under $20), coffee houses, carry out and take away, bars, and more expensive restaurants ($20-$50)

(2) Jupyter file : prompt.ipynb (link : https://github.com/anandtongle7/BKML/blob/main/Assignment1/prompt.ipynb)
This jupyter file provides a code to analyzes the data selected and provides detaied visualization on such analysis.
There are two types of Coupon data analyzed in the jupyter program
  a. Bar Coupons
  b. Coffee House Coupons 

The analsysis aims at determining the acceptance rate of the above coupons by the customers based on collected data

Summary of analysis is as follows: 
  (1)  BAR coupon acceptance rate is 
       #1# Highest among drivers who are above the age of 25 and below 35 years of age 
       #2# High acceptance rate among the drivers who visit Bar atleast once a month and highest among those visit more than 3 times a month
       #3# Rate is almost 1/2 if the driver is accompanying the kids 
       #4# Less than 1/2 if we know that the drivers have been visiting resturants less than 4 times a month & has income less than 50K

  (2) Coffee Coupon acceptance rates are high in 
       #1# When weather is Sunny 
       #2# Passanger class which has friends specially in the age class of 26 and 41 
       #3# Most of the time, these high coffee acceptaor friend passanger class are single friends or unmarried partners 
       #4# Also found out that coffee coupon acceptance is high in income class which is > 1 Mil and < 12.5K and suprisingly, males use more of the coffee coupons as compared to females
       #5# Coffee coupon usage is also high in specific occupation classes like Architecture & Engineering, Healthcare Support and Production Occupations and makes again dominate in using the coffee coupons as compared to females


