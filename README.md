# Customer-Retention-Churn-Analysis-Project

Project Overview
This project analyzes customer churn and retention behavior using a telecom subscription dataset. The objective was to identify "why customers are leaving", "which segments are most at risk", and "how retention impacts revenue", and then translate these findings into actionable business strategies.
The dashboard is structured to simulate a real-world business scenario, where insights directly support "product, pricing, and retention decisions".


Business Problem
Customer churn is a major challenge in subscription-based businesses.

This project answers:
* Why is churn happening?
* Which customers are most likely to churn?
* When do customers churn in their lifecycle?
* How does retention affect revenue (CLV)?
* What actions can reduce churn?


Tools & Technologies
* Power BI → Dashboard creation & storytelling
* Python (Jupyter Notebook) → Data cleaning & preprocessing
* DAX → Measures, KPIs, segmentation

Data Cleaning & Preparation (Python)
The dataset was preprocessed using Python before visualization:
* Converted "tenure and numerical fields" into correct data types
* Handled missing values and inconsistencies
* Standardized categorical values (e.g., contract types, services)
* Created derived features:
  * Churn Flag (1 = Yes, 0 = No)
  * Tenure Groups (0–12, 12–24, 24–48, 48+)
  * Risk Segmentation (High / Medium / Low)
This ensured the dataset was analysis-ready and consistent across all visuals.

Dashboard Structure
1. Churn Overview & Drivers (WHAT + WHY)
Provides a complete view of churn patterns and root causes:

* KPIs:
  * Total Customers → **7,043**
  * Churned Customers → **1,869**
  * Active Customers → **5,174**
  * Churn Rate → **26.54%**
  * Avg Tenure → **32.37 months**

* Churn Distribution:
  * Month-to-month → **42.71% churn**
  * One-year → **11.27%**
  * Two-year → **2.83%**

* Tenure-Based Churn:
  * 0–12 months → **47.68% (highest churn)**
  * 12–24 months → **28.71%**
  * 24–48 months → **20.39%**
  * 48+ months → **9.51%**

* Service-Level Drivers:
* Fiber Optic → **42% churn**
* DSL → **19%**
* No Internet → **7%**
* Tech Support:
    * No → **42% churn**
    * Yes → **15%**
* Online Security:
    * No → **42% churn**
    * Yes → **15%**

* Payment Behavior:
  * Electronic Check → **45% churn (highest)**
  * Mailed Check → **19%**
  * Bank Transfer → **17%**
  * Credit Card → **15%**

* Risk Segmentation:
  * Low Risk → **4.9K customers**
  * High Risk → **1.4K customers**
  * Medium Risk → **~0.8K customers**

2. Retention & Customer Lifecycle (WHEN + VALUE)

* Retention Trend:
  * Strong drop in early tenure, stabilizes after ~12 months

* Churn Trend:
 * Peaks early (~0.62) and declines steadily to ~0.02

* Tenure Distribution:
  * 0–12 → **2,175 customers**
  * 12–24 → **1,024**
  * 24–48 → **1,594**
  * 48+ → **2,239**

* Average Tenure by Contract:
  * Two-year → **57 months**
  * One-year → **42 months**
  * Month-to-month → **18 months**

* Customer Lifetime Value (CLV):
  * Two-year → **6.3M (highest)**
  * Month-to-month → **5.3M**
  * One-year → **4.5M**

* Customer Segmentation Heatmap:
   * Highest concentration:
     * Month-to-month + 0–12 months → **1,994 customers**
  * Long-tenure dominance:
    * Two-year + 48+ months → **1,263 customers**


3. Key Insights
* **26.54% churn rate** indicates a significant retention issue
* **Month-to-month contracts (42.71%)** are the biggest churn driver
* Majority of churn happens in **early lifecycle (0–12 months: 47.68%)**
* Lack of **Tech Support and Online Security (~42% churn)** significantly increases risk
* **Fiber users (42%)** show higher churn, indicating pricing/value mismatch
* Long-term customers (2-year) show:

  * Highest retention (**57 months**)
  * Highest revenue contribution (**6.3M CLV**)


4. Recommendations & Business Actions
* Encourage long-term plans through incentives and bundled offers
* Improve onboarding experience to reduce early churn
* Bundle support and security services into core plans
* Target **1.4K high-risk customers** proactively
* Re-evaluate pricing and service quality for fiber users
* Improve payment experience (reduce reliance on electronic checks)


Business Impact
This analysis enables:
* Reduction in early-stage churn through targeted onboarding
* Identification of high-risk segments for proactive retention
* Improved revenue via increased customer lifetime value
* Better product bundling strategies (support + security)
* Shift from reactive churn handling to proactive retention strategy

Key Takeaway
Customer churn is primarily driven by:

* **Low commitment (month-to-month plans)**
* **Poor early experience (0–12 months)**
* **Lack of service support**

Improving these areas can significantly enhance retention and long-term revenue.


