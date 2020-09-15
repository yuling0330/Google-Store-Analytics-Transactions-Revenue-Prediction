# Google Store Analytics Transactions Revenue Prediction
---
### Background

**Industry Overview**: The e-commerce market has changed the way business is transacted, whether in retail or business-to-business. The e-commerce market has become such a vital part of the economy that is difficult to pinpoint exactly where e-commerce begins and the old world economy ends. One of the largest segments of e-commerce is the online retail sector, which is dominated by the sale of consumer electronics, apparel and accessories. 

**Google Store**: The Google Merchandise Store is an ecommerce site that sells Google-branded merchandise from accessories, bags, clothes to office related supplies. With is wide range of products, it can be difficult to understand and track customers needs. 

---
### Problem Statement:

The 80/20 rule has proven true for many businesses, only a small percentage of customers produce most of the revenue. 
Understanding how much each customer spends will allow companies to place actionable operations 
to better allocate their 
marketing budgets.

---
### Objective:

Predict a how much GStore customer will spend. In addition, to predict the natural log of the sum of all transactions per user.

<p align="center">
  <img src="https://github.com/yuling0330/Google-Store-Analytics-Transactions-Revenue-Prediction/blob/master/image/formula.PNG" />
</p>

---
### Data:

- fullVisitorId- A unique identifier for each user of the Google Merchandise Store.
- channelGrouping - The channel via which the user came to the Store.
- date - The date on which the user visited the Store.
- device - The specifications for the device used to access the Store.
- geoNetwork - This section contains information about the geography of the user.
- socialEngagementType - Engagement type, either "Socially Engaged" or "Not Socially Engaged".
- totals - This section contains aggregate values across the session.
- trafficSource - This section contains information about the Traffic Source from which the session originated.
- visitId - An identifier for this session. This is part of the value usually stored as the _utmb cookie. This is only unique to the user. For a completely unique ID, you should use a combination of fullVisitorId and visitId.
- visitNumber - The session number for this user. If this is the first session, then this is set to 1.
- visitStartTime - The timestamp (expressed as POSIX time).
- hits - This row and nested fields are populated for any and all types of hits. Provides a record of all page visits.
- customDimensions - This section contains any user-level or session-level custom dimensions that are set for a session. This is a repeated field and has an entry for each dimension that is set.
- totals - This set of columns mostly includes high-level aggregate data.

 (ps: train_v2.csv.zip and test_v2.csv.zip is used)
 
 ---
 ### References:
 - *Data Source is from Kaggle: https://www.kaggle.com/c/ga-customer-revenue-prediction/data*
