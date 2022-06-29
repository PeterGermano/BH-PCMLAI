# Coupon Data and Review

Will a Customer Accept the Coupon?

Context

Imagine driving through town and a coupon is delivered to your cell phone for a restaraunt near where you are driving. Would you accept that coupon and take a short detour to the restaraunt? Would you accept the coupon but use it on a sunbsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaraunt? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day?

Obviously, proximity to the business is a factor on whether the coupon is delivered to the driver or not, but what are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

Overview

The goal of this project is to use what you know about visualizations and probability distributions to distinguish between customers who accepted a driving coupon versus those that did not.

Data

This data comes to us from the UCI Machine Learning repository and was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. Answers that the user will drive there ‘right away’ or ‘later before the coupon expires’ are labeled as ‘Y = 1’ and answers ‘no, I do not want the coupon’ are labeled as ‘Y = 0’. There are five different types of coupons -- less expensive restaurants (under $20), coffee houses, carry out & take away, bar, and more expensive restaurants ($20 - $50)

Findings

Overall, approximately 57% of drivers acceted a coupon. Acceptance of the coupon varied by location, with most accepted coupns for carry out & takeaway and less expensive restaurants. While bar coupons were not accepted as readily, approx. 41% of the coupons were still accepted. Furthur analysis of bar coupons found that coupons were more readily accepted, closer to 70%, by those who visited a bar more than once a month. The increased percentage appears to be independant of covariants like age, passenger or occupation. Coffee Houses had an even ratio of drivers accetping and not accepting coupons (50%/50%). When examined together, the weather and time of day combined to be factors in the acceptance of coupons. One examlple is on rainy mornings, 68% of coupons were accepted compared to rainy evenings where only 38% were accepted.  Additional stratification of the weather and time dependence should be explored to understands it relationship to coupon acceptance in other tpyes of locations. 

