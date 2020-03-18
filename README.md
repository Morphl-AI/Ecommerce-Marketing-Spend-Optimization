# Marketing Spend Optimization for Online Retailers
## 1. Introduction 

The task is to optimize the budget allocation between multiple campaigns.Some of them are "inner" optimizable (Google Ads, Facebook Ads), others are out of reach: E-mail, SEO, etc. There are multiple "problems" at once that are embedded in this "budget allocation" term and we’ll try to provide a direction to solving the problem using the campaigns as black-boxes, making use only of the cost and the revenue produced.

## 2. Budget Allocation Overview

First of all, in the perfect scenario, where we got a set of Campaigns {C1, ..., Cn} with a perfectly
explainable function Budget(i) → Revenue(i), for i ∈ Campaigns, the task is trivial to solve (Appendix
A). However, campaigns are most likely not a linear function of Budget, meaning that investing too
little or too much would cause non-linearities.

The main issue here is that there are some hard assumptions about the Projected Revenues,
which are probably hand picked. We’ve got a small time series and we can know for
each day (Google Ads Daily/Facebook Ads Daily) and monthly how much we invested and how much revenue we got. 

We can, thus, predict how much the daily/monthly revenue we'll have, given the historical data. This will automatically give a model where we can predict for each campaign and given budget an estimated revenue return.

Another observable fact is that picking the weights for all campaigns relatively close to each
other {0.2857, 0.3174, 0.3968}, meaning putting all eggs
in one basket (best performing one), is wrong. We could alter the weights to be close to each other
using a regularization technique, while also allowing favouring the best performing one.

Thus, the task is divided into 2 parts.
• Computing a model (B → Rev) for each Campaign
• Compute a optimal budget allocation, given the models for each Campaign

### 2.1 Time Series Model
...
### 2.2 Optimal Optimization Problem
...

