# Project Portfolio: Implementing the UCB Algorithm for Ads Click-Through Rate Optimization

**Author:** Malick H.B

## Introduction

In the realm of online advertising, optimizing the click-through rate (CTR) is pivotal for enhancing the effectiveness of ad campaigns. This project revolves around the utilization of the Upper Confidence Bound (UCB) algorithm to optimize ad selections, thereby maximizing CTR. By working with the "ads_CTR_customers" dataset from Kaggle, we explore the steps involved in implementing the UCB algorithm, explaining both the process and the accompanying code.

## Dataset Overview

The "ads_CTR_customers" dataset furnishes simulated click-through rate data for various ads exhibited to customers. Each record corresponds to a customer's interaction with a specific ad, including details such as customer ID, ad ID, ad click status, and more. The primary goal of the project is to leverage this data to ascertain the optimal ads to display to customers in order to maximize the aggregate click-through rate.

## Upper Confidence Bound (UCB) Algorithm

The UCB algorithm stands as a prominent solution for addressing the exploration-exploitation trade-off in multi-armed bandit problems. In the context of ad selection, the UCB algorithm strikes a balance between displaying ads that demonstrate favorable performance (exploitation) and exploring new ads in the hope of discovering even better-performing ones (exploration). The algorithm estimates the expected reward (CTR) for each ad and computes a confidence bound that captures the uncertainty in this estimate. Subsequently, the ad with the highest upper confidence bound is chosen for presentation to the next customer.

## Data Preprocessing

- Importing essential libraries: NumPy, pandas, Matplotlib.
- Loading the dataset: Utilized `pd.read_csv()` to load the "ads_CTR_customers" dataset.
- Inspecting the dataset: Displayed the initial rows of the dataset and its shape.
- Dataset dimensions: The dataset comprises 10,000 rows and 10 columns.

## Implementing the UCB Algorithm

- Initialization: Variables were initialized to monitor the number of times each ad was displayed (`numbers_of_selections`) and the cumulative reward received for each ad (`sums_of_rewards`).
- Looping through customers: A loop iterated through each customer's interaction.
- Choosing the ad: For each customer, the ad with the highest upper confidence bound was chosen using a nested loop.
- Updating variables: The selected ad's information and rewards were updated for future iterations.
- Calculating click-through rate: The total clicks and click-through rate were calculated and printed.

## Visualizing the Results

- Histogram: The selections of each ad were visualized through a histogram.

## Conclusion

The implementation of the UCB algorithm showcased its effectiveness in optimizing ad selections for click-through rate enhancement. By analyzing the results, it was evident that "Ad 5" had the highest number of selections and cumulative rewards, indicating the highest click-through rate. Consequently, "Ad 5" was deemed the most attractive to customers, substantiating its potential for future ad campaigns. This project exemplifies the power of the UCB algorithm in making informed decisions in the realm of online advertising.
