# Custom Mobile App Usage Behavior Segmentation for Telecom Industry


## Introduction
Just because one user consume most of their data in a particular mobile app, that doesn't necesarily mean that he likes the app, nor that he is willing to pay for services related to the apps he consume most.

For that purpose it is necessary to compare the user with other users and give him a "score", then we can determine if his app consumtion is relevant (compared with others) or just normal.


- This work is divided in three parts:

    1. Sampling: to prepare the data for analysis.
    2. Feature engineering:  
        - Features generated: traffic, duration and session frequency. 
        - Quantile discretization was made to the features (general and by category app) to spot in what categories the users stand out the most.
    3. Clustering: to group similar users and spot potential patterns.

## The Dataset

"Tsinghua App Usage Dataset"
Yu, D., Li, Y., Xu, F., Zhang, P., & Kostakos, V. Smartphone app usage prediction using points of interest. Proceedings of the ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies (ACM IMWUT/UbiComp), 1(4), 174, 2018.

http://fi.ee.tsinghua.edu.cn/appusage/


|Dataset files|Description|
|---|---|
| App_usage_trace.zip | User ID, Timestamp(Second), Location (base station ID), Used App ID, Traffic (Byte) |
| App2Category.zip | App ID, Category ID|
| Categorys.zip| Category ID, English Name|

## The Dashboard
The data processing produce a friendly format to plot the results in any BI tool (such as Power Bi, Tableau, Google Data Studio etc.).
Note: the dataset used for the dashboard was mainly the "QUANTILIZED_table_stacked_format_S6Q5.csv" dataset.

Here an example in Google Data Studio:
- https://datastudio.google.com/reporting/72a89cb6-1136-4800-9f2e-329a7e1d6475
