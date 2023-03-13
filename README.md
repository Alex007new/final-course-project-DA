# final-course-project-DA

This is an academic project, implemented by us as a final project, upon completion of the Data Analyst course (educational resource https://karpov.courses).
In the course of the project, we used exploratory data analysis, parametric and nonparametric methods, bootstrapping, correlation analysis, multivariate  analysis of variance, ect.

**The introductory information is as follows:**

Imagine that you work for a large dating app.

In addition to the basic functions, the application also has a premium subscription, which gives you access to a number of important additional features. An A/B test was conducted, in which for new users from several countries, the cost of a premium subscription * was changed when buying through two new payment systems. At the same time, the cost of the trial period remained the same.

_*Subscription money is charged monthly until the user cancels it._

**Check:**
  1) Was the experiment successful overall?
  2) Analyze whether the innovation makes sense among any specific user groups?

**Data**\
There are three groups in total: test (**test**), control 1 (**control_1**), control 2 (**control_2**).\
For each of them:

**users_*.csv** - information about users:\
        **uid** - user ID;\
        **age** - age;\
        **attraction_coeff** – attraction coefficient (from 0 to 1000, (likes / views) * 1000);\
        **coins** - number of coins (local currency);\
        **country** - country;\
        **visit_days** - on which days after registration the user visited the application (for example, at 1, then at 7);\
        **gender** - gender;\
        **age_filter_start** – search filter, min. meaning;\
        **age_filter_end** - search filter, max. meaning;\
        **views_count** - number of views received;\
        **was_premium** - whether there was ever a premium (either a trial period of premium status, or bought for money);\
        **is_premium** - whether premium;\
        **total_revenue** - normalized revenue.
 
**transactions_*.csv** – information about user payments:\
        **uid** - user ID;\
        **country** - country;\
        **joined_at** - date and time of registration;\
        **paid_at** - date and time of purchase;\
        **revenue** - normalized revenue;\
        **payment_id** - payment ID;\
        **from_page** - from where the user went to the payment page;\
        **product_type** - product type (_trial_premium_ - trial premium subscription, _premium_no_trial_ - premium subscription without trial, _coins_ - subscription for local currency, _other_type_ - other).
 
**Files:**

**users_test** - information about users in the test group;\
**users_control_1** - information about users in the first control group;\
**users_control_2** - information about users in the second control group;\
**transactions_test** - information about user payments in the test group;\
**transactions_control_1** – information about user payments in the first control group;\
**transactions_control_2** - information about user payments in the second control group.

