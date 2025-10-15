# nicobar-proxy-omni-channel
The project demonstrates how analytical frameworks from retail can be adapted for lifestyle brands like Nicobar, linking customer segmentation, CLV, product affinity, and engagement analytics to brand strategy and CRM design.

# Omnichannel Customer Segmentation and Insight Framework
## *Translating Grocery Retail Analytics to Lifestyle Brand Strategy (Nicobar Case)*

## Executive Summary
This project demonstrates how data-driven retail analytics can be applied beyond traditional grocery retail, into the world of premium lifestyle and design brands like Nicobar. 

Using open-source omni-channel grocery datasets and synthetically derived customer data, I designed an analytical framework covering customer segmentation, channel performance, CLV modelling, and engagement strategy. 

The goal: to show how quantatitive insights can inform emotional brand storytelling, CRM personalisation, and omnichannel experience design, helping brands like Nicobar balance community, commerce, and creativity. 

## Problem Statement
While lifestyle and design-led brands often focus on creative storytelling, there's a growing need to integrate data intelligence into brand growth strategy, without losing authenticity. 

The challenge is to create a system that answers:
- Who are our core and emerging customer segments?
  
- How do their behaviours differ across channels (online vs in-store)?

- WHich clusters drive long-term value versus short-term sales?

- How can engagement and loyalty be cultivated beyond discount-driven models?

This project using grocery retail data as a proxy sandbox to simulate these questions in a structured, data-backed way. 

# Data Sources and Engineering

## Data Sources:
Four open-source datasets were sourced from GitHub's repository:
1. **Product Family Mapping** :- served as the foundation for synthetically generating the Customer dataset.

2. **Product Information** - provided product hierarchy and category relationships.

3. **Demand and Shopping Behaviour** - captured purchase patterns and spend behaviour across categories.

4. **In-store and Online Customer Arrivals** - reflected channel traffic and visit frequency patterns.

All other analytical dataframes - including customers_master, revenue_by_cluster, marketing_effectiveness, product_affinity, and cly_proxy, were engineered from these core files using Python. 

## Engineering:
- Merged and standardised all data sources into a master analytical base.

- Performed feature scaling, encoding, and normalisation for segmentation readiness.

- Created synthetic customer records derived from product mapping and engagement data.

- Engineered key KPIs such as churn score, loyalty score, engagement index, and online purchase ratio.

- Conducted outlier detection, missing value treatment, and normalisation via Scikit-learn StandardScaler.

# Methodology
1. **Data Preparation and Standardisation** : Combined raw and synthetic datasets, cleaned and encoded categorical variables.

2. **Segmentation and CLustering** : Applied K-Means clustering (K=5) optimised via tha Elbow and Silhouette method to form behavioural segments.

3. **Cluster Profiling** : Labeled clusters based on loyalty, engagement, spend, and visit frequency to derive five behavioral personas:

   - Enagegd Regulars
  
   - Transitional Shoppers
  
   - Premium but At-Risk
  
   - Occasional Premiums
  
   - Price-Sensitive Shoppers
  
4. **Revenue, CLV and Marketing Analysis** : Calculated revenue share, customer lifetime value (CLV proxy), and churn risk per cluster.

5. **Operational and Channel Efficiency** : Studied dwell time, basket size, and online vs. in-store ratio to identify cross-channel optimisation levers.

6. **Product Affinity and Engagement Journey** : Analysed cross-category preferences and engagement index to derive actionable cross-sell and personalisation insights.

7. **Visualisation and Reporting** : Synthesized insights into a strategic deck and Power BI dashboard, bridging retail analytics and brand strategy.

# Key Findings and Impact

**From Grocery Retail Insights to Nicobar Opportunities** 

| **Analytical Lens**         | **Key Finding (Grocery)**                                | **Strategic Relevance for Nicobar**                                |
|:----------------------------:|:--------------------------------------------------------:|:------------------------------------------------------------------:|
| **Customer Segmentation**   | 5 distinct behavioral clusters identified                | Define Nicobar personas: Loyalists, Explorers, Occasionals, At-Risk |
| **Revenue Drivers**         | High-value but low-frequency buyers drive 30% of revenue | Plan micro-collections and CRM nudges between drops                 |
| **Marketing Effectiveness** | Loyalty linked to frequency, not spend                   | Build community-based loyalty programs                              |
| **Operational Efficiency**  | Avg. dwell time ~19 mins, basket ~7 items                | Measure “brand immersion” time across store & site                  |
| **Product Affinity**        | Emotional + habitual category pairs dominate             | Curate collections by intent (Hosting, Comfort Living)              |
| **Customer Lifetime Value** | Highest CLV in *Occasional Premiums*                     | Focus on experiential retention — not discounting                   |
| **Competitive Positioning** | 25% At-Risk, 24% Potential Loyalists                     | Prioritize win-back and personalized reactivation                   |

# Tools and Technologies

| **Category**                  | **Tools / Libraries**                                     |
|:------------------------------:|:---------------------------------------------------------:|
| **Programming**               | Python (Pandas, Scikit-learn, Seaborn, Matplotlib) |
| **Visualization**             | Power BI, Matplotlib, Seaborn                             |
| **Modeling**                  | K-Means Clustering, PCA                                   |
| **Data Engineering**          | Feature Scaling, Encoding, Synthetic Data Generation      |
| **Documentation & Reporting** | Google Colab Notebook, Canva, MS Word             |

# Visualisations

1. **Customer Segmentation Overview** : Visualises 5 behavioural clusters with PCA reduction, representing distinct spend, frequecy, and engagement patterns.
   
   ([Scatter Plot](https://github.com/aarushijain16/nicobar-proxy-omni-channel/blob/main/PCA.png), [Bar Graph](https://github.com/aarushijain16/nicobar-proxy-omni-channel/blob/main/Customer%20Segmentation%20Overview.png))

2. [**Revenue Contribution by Cluster**](https://github.com/aarushijain16/nicobar-proxy-omni-channel/blob/main/Revenue%20Contribution.png) : Highlights clusters driving the largest share of total revenue.

3. [**Marketing Effectiveness Scatter**](https://github.com/aarushijain16/nicobar-proxy-omni-channel/blob/main/Loyalty%20vs%20Churn.png) : Compares churn risk and loyalty index across clusters, a lens into retention opportunities.

4. [**CLV Proxy by Cluster**](https://github.com/aarushijain16/nicobar-proxy-omni-channel/blob/main/CLV%20Proxy.png) : Identifies the most valuable segments (highest CLV among Occasional Premiums).

5. [**Product Affinity Composition**](https://github.com/aarushijain16/nicobar-proxy-omni-channel/blob/main/Product%20Affinity.png) : Displays dominant product categories by cluster, showing lifestyle parallels for Nicobar.

6. [**Operational Efficiency**](https://github.com/aarushijain16/nicobar-proxy-omni-channel/blob/main/Operational%20Efficiency.png) : Demonstrates consistent dwell patterns and category engagement, relevant for store flow and UX mapping.


# Final Note
This project represents the intersection of data science, strategy, and storytelling, translating structured analytic into creative business impact. 

It reflects how omnichannel insights, even from synthetic or non-fashion data, can shape personalisation, retention, and emotional connection for a modern lifestyle brand. 
