# Customer Segmentation Using Kmeans
This is a learning project where I explored an e-commerce dataset and applied K-Means clustering for customer segmentation.

The data that I used in this project: https://archive.ics.uci.edu/dataset/502/online+retail+ii.

## 1. Executive Summary

This project analyzes customer transaction data to segment the customer base using **RFM** (Recency, Frequency, Monetary) analysis and clustering techniques. The results reveal that while the company excels at attracting new customers, there is a clear opportunity to improve customer retention and conversion into high-value loyal segments.

**Key highlights:**

- The **Promising** segment is the largest, representing many recent buyers with strong potential for long-term loyalty.
- The **At Risk** segment is also large, signaling possible churn among previously engaged customers.
- **Loyal Customers**, **Champions**, and **Very Loyal Customers** form a small share of the base, indicating low progression from new buyers to top-tier loyalty.

These insights provide a foundation for targeted marketing strategies to improve retention, increase customer lifetime value (CLV), and optimize acquisition investments.

---

## 2. Methodology Overview

### 2.1 Data Preparation
- **Data Cleaning:** Removed invalid transaction entries, handled missing values, standardized formats.
- **Feature Engineering:** Computed RFM scores (Recency, Frequency, Monetary value) for each customer.
- **Scaling:** Normalized values for clustering using `StandardScaler`.

### 2.2 Segmentation Approach
- **Clustering:** Applied K-Means clustering to identify customer segments.
- **Validation:** Used silhouette scores and inertia values to determine the optimal number of clusters.

### 2.3 Segment Labeling
- Segments were mapped to known customer behavior archetypes using the RFM segmentation reference table (e.g., Champions, Loyal Customers, At Risk, Promising, Lost, etc.).

---

## 3. Key Insights

1. **Promising customers (~1,600)** → Many recent buyers with high potential but not yet fully loyal.  
2. **At Risk customers (~1,250)** → Significant portion whose activity has dropped; high churn risk.  
3. **Potential Loyalists (~1,050)** → Good pipeline of customers close to becoming loyal if nurtured.  
4. **Loyal Customers, Champions, Very Loyal Customers** → Small share of total base; low retention.  
5. **Lost customers (~700)** → Could be reactivated but may have low ROI unless strategically targeted.

---

## 4. Implications

- **Strong acquisition:** The company is effective at bringing in new customers.  
- **Retention gap:** Low conversion from early-stage segments (Promising, Potential Loyalists) into Loyal or Champion tiers.  
- **Churn risk:** High At Risk numbers suggest engagement drops after initial activity.

---

## 5. Recommended Actions

1. **Promising → Loyal Conversion**  
   - Launch onboarding and nurture campaigns with personalized offers.  
   - Use time-limited discounts to drive quick follow-up purchases.  

2. **At Risk Win-back**  
   - Send targeted reactivation campaigns with strong incentives.  
   - Collect feedback to address churn drivers.  

3. **Strengthen Loyalty**  
   - Enhance loyalty programs for top segments.  
   - Offer VIP perks and personalized rewards.  

4. **Lost Customer Strategy**  
   - Re-engage selectively based on CLV potential.  
   - Focus on high-likelihood returnees over broad campaigns.  


**REFERENCE:**
Kansal, T., Bahuguna, S., Singh, V., & Choudhury, T. (2018). Customer Segmentation using K-means Clustering. 2018 International Conference on Computational Techniques, Electronics and Mechanical Systems (CTEMS). 
