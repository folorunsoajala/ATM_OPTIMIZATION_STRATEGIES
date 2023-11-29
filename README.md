# ATM OPTIMIZATION STRATEGIES
![](atm.png)
---
## Introduction

In the ever-changing landscape of banking today, maintaining customer loyalty has become a crucial factor for the success of financial institutions. The ability to keep devoted customers has a direct impact on profitability, market share, and brand reputation. One key interaction point with customers is the **Automated Teller Machine (ATM)**, which remains a fundamental channel for cash withdrawal and various banking transactions. Recognizing the significance of customer retention, we are initiating a transformative Business Intelligence and Data Analytics project. The goal is to explore data-driven strategies to optimize ATM performance, ultimately leading to improved customer retention. Through the utilization of data analytics, our objective is to uncover valuable insights that will enhance our understanding of customer behavior, boost operational efficiency, and foster enduring customer relationships.

![](objective.jpeg)
## Objectives 
With the power of data analytics and a customer-centric approach, this project aspires to empower financial institutions with the tools to make informed decisions that drive customer retention and loyalty. By optimizing ATM performance, banks can not only improve operational efficiency but also deliver an exceptional customer experience that nurtures lasting relationships and positions them for sustained success in today's competitive financial landscape.
- Identify Factors Affecting Customer Retention
By analyzing transaction data and customer feedback, I aim to pinpoint factors that impact customer retention, such as transaction success rates, wait times, and customer experience.
-  Analyze ATM Usage Patterns
I will delve into the patterns of ATM usage, identifying peak hours, days, and seasonal trends. Understanding when and how customers engage with ATMs is pivotal to optimizing service availability and ensuring customer satisfaction.
- Evaluate ATM Performance
 Assessing the performance of individual ATMs and comparing performance across different locations will help us identify areas of improvement and prioritize resource allocation.
- 	Optimize ATM Servicing and Maintenance 
By evaluating maintenance schedules and correlating them with ATM performance, we can optimize servicing to prevent downtime and disruptions.
---
![](architeture.png)
---
## Tool use 
In this project, we will leverage the power of Microsoft SQL Server, Microsoft Power BI Desktop, and Microsoft Fabric to efficiently manage and analyze data. The primary data source for this project is the **datakliq_education_hub** specifically, their Cohort 3 project dataset.

### Dataset Description:
The dataset comprises a collection of dimension tables, including Customer, ATM Maintenance, Calendar, ATM Location, Hour, and Transaction Type. Additionally, there is one fact table named "Transaction Table," which contains a multitude of transactions spanning five different states in Nigeria. These states are Lagos, Enugu, FCT (Federal Capital Territory), Rivers, and Kano.

### Data Dictionary:
To ensure clarity and understanding, we have access to a meticulously defined data dictionary. This resource provides comprehensive explanations for the table and column structures, aiding our data analysis process.

## Data transformation 
Most of my data transformation processes were executed on Microsoft SQL Server. In these processes, I performed tasks such as appending data, generating new calendar tables, creating a bridge table to link the transaction table with the maintenance table, and employing the alter and update functions to modify specific tables, as depicted in the screenshot below.

Example1              |   Example2
:---------------------| :----------------------:
![](transform1.png)   | ![](transform2.png)

# Data Modelling 
I implemented the snowflake model, connecting all my facts and dimensions seamlessly. I utilized the import storage mode to bring in my data into Power BI, where I established relationships. The majority of these relationships have a one-to-many cardinality, and a single filter direction was applied, as illustrated in the screenshot below.

Snowflakeschema          |Relationship      
:---------------------| :----------------------:
![](model1.png)   | ![](model2.png)

