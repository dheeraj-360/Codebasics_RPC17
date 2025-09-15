# Bharat Herald – Digital Transformation Analysis 📊

## 📌 Problem Statement
Bharat Herald, a 70-year-old newspaper, is facing an existential crisis in a **post-COVID digital era**.  
Between **2019 and 2024**, print circulation dropped from **1.2M → 560K**.  
Competitors quickly adapted with **mobile-first platforms, WhatsApp delivery, and subscriptions**, but Bharat Herald’s 2021 digital pilot failed due to poor usability.  

This project analyzes Bharat Herald’s **operational, revenue, and digital performance data** to:  
- Quantify what went wrong  
- Identify recovery opportunities  
- Recommend a phased roadmap for **digital transformation**

---

## 🚀 Project Deliverables
1. **Power BI Dashboard** with 3 key views:
   - **Overall Performance** – circulation, wastage, profitability
   - **Revenue Analysis** – advertiser trends, revenue per copy
   - **Digital Performance** – readiness, engagement, bounce rates
2. **Strategic Insights & Recommendations**
3. **Presentation (PPT)** for stakeholders

---

## 📊 Key Insights
- 📉 **Steady Decline** – Copies printed & circulated fell sharply (2019–2024)  
- 📰 **Wastage %** – Delhi (10.71%), Ahmedabad (10.67%), Varanasi (10.43%) highest  
- 💰 **Revenue per Copy** – Ranchi, Ahmedabad, Patna lead (>₹10/copy)  
- 🏆 **Most Profitable City (2024):** Lucknow  
- 📢 **Advertiser Spend** – 59% from Government + Real Estate  
- 🌐 **Digital Performance** – ₹12.2M investment, 683K engagement, bounce rate **65.7%**  
- 📱 **Best Digital Platform:** Mobile App Beta (61.83% engagement)  
- ⚠️ **Kanpur Outlier:** High readiness (75.1) but **very low engagement (38.5₹/user)**  

---

## 📌 Recommendations & Strategy
1. **Phased Digital Transition**  
   - Phase 1: Relaunch in **Kanpur, Ranchi, Patna** (high readiness but poor engagement)  
   - Phase 2: Expand to **Ahmedabad, Delhi, Mumbai** (balanced reach + ROI)  

2. **Regain Advertiser Trust**  
   - Showcase **ROI metrics** (Revenue per Copy & Cost per User)  
   - Bundle print + digital packages for key industries (Govt., Real Estate, FMCG)  

3. **Boost Digital Engagement**  
   - Launch **WhatsApp bulletins** & **mobile-optimized e-papers**  
   - Improve UI/UX to reduce bounce rate  

4. **Revenue Recovery Models**  
   - Subscription bundles (Print + Digital)  
   - Pay-per-article & loyalty programs  

5. **Local Market Strategy**  
   - Collaborate with **regional influencers/journalists**  
   - Localized content to build digital credibility  

---

## 🛠️ Tools Used
- **Power BI** – Interactive dashboards  
- **Excel & SQL** – Data cleaning & calculations  
- **MS PowerPoint** – Storytelling & presentation


## Some Important DAX Measures Created

-- Digital Readiness Score

Digital_Readiness_Score =
(AVERAGE(fact_city_readiness[literacy_rate])+ AVERAGE(fact_city_readiness[smartphone_penetration])+AVERAGE(fact_city_readiness[internet_penetration])) / 3

-- Engagement Rate

Engagement Rate =
DIVIDE(SUM(fact_digital_pilot[downloads_or_accesses]),
       SUM(fact_digital_pilot[users_reached]), 0)

-- Cost per User

Cost_Acquired_Per_User =
DIVIDE(SUM(fact_digital_pilot[dev_cost] + fact_digital_pilot[marketing_cost]),
       SUM(fact_digital_pilot[downloads_or_accesses]), 0)

-- Revenue per Copy

Revenue_Per_Copy =
DIVIDE(SUM(fact_ad_revenue[ad_revenue]),
       SUM(fact_print[copies_circulated]), 0)

-- Print Decline %

Print_Decline% =
DIVIDE((MAX(fact_print[copies_circulated]) - MIN(fact_print[copies_circulated])),
       MAX(fact_print[copies_circulated]), 0)

---

## 📷 Dashboard Preview
**Overall view**
<img width="1333" height="747" alt="image" src="https://github.com/user-attachments/assets/30343ff6-c945-4e5f-a07e-b2a3c0322745" />
**Revenue Analysis**
<img width="1332" height="751" alt="image" src="https://github.com/user-attachments/assets/f6885db5-ca6d-45a8-90ce-636e4831c4bc" />
**Digital Performance(2021)**
<img width="1331" height="753" alt="image" src="https://github.com/user-attachments/assets/3af53746-82c0-4327-bef7-5e9364b875cc" />
**Data Modelling**
<img width="1371" height="749" alt="image" src="https://github.com/user-attachments/assets/9b408cb5-29c8-4500-a072-92659be14a14" />





---


