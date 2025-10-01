##  Project: Hypothesis Prioritization and A/B Test Analysis

---

### **Objective**

To optimize a major online retailer's revenue stream through a two-step analytical process:
1.  **Strategic Prioritization:** Evaluate and rank nine revenue-boosting hypotheses using the **ICE** and **RICE** frameworks to define the optimal product roadmap.
2.  **A/B Test Validation:** Conduct a comprehensive analysis of an ongoing A/B test using **statistical methods** (Mann-Whitney U Test) to make a definitive, data-driven decision on whether to stop the test and implement the new feature.

---

### **Results**

* **Final A/B Test Decision:** The test was deemed complete and **STOPPED**. **Group B was declared the winner** due to a significant positive effect on the primary business metric.
* **Primary Metric Impact:** Statistical analysis on the cleaned data showed a **statistically significant uplift** in the **Conversion Rate (CR)** for Group B.
* **Secondary Metric Impact:** The **Average Order Value (AOV)** difference between the groups was **not found to be statistically significant**.
* **Prioritization Shift (ICE vs. RICE):** The inclusion of the **Reach** factor in RICE changed the strategic focus. The RICE framework prioritized the hypothesis with the **broadest audience reach** (e.g., adding a universal subscription form) over ideas with high but narrow impact (e.g., a specific promotion), guiding future development toward scalability.
* **Data Integrity:** The final results were obtained only after successfully identifying and removing **cross-group user contamination** and **high-impact revenue/order outliers** (anomalies) from the data.

---

### **Tools**

* **Python**
* **Pandas** (Data cleaning, aggregation, cumulative metrics calculation, and outlier filtering using percentiles like P95/P99)
* **NumPy** (Numerical operations)
* **Matplotlib & Seaborn** (Cumulative metric plotting and distribution visualization)
* **SciPy** (Statistical testing, specifically the **Mann-Whitney U Test**)

---

### **Skills Learned**

* **Hypothesis Prioritization:** Applying and contrasting the **ICE and RICE** frameworks to build a strategic product roadmap.
* **A/B Test Data Integrity:** Detecting and eliminating **data contamination** (users in both groups) and performing **outlier analysis** to ensure test reliability.
* **Statistical Validation:** Applying the **Mann-Whitney U Test** to determine the statistical significance of differences in Conversion Rate and AOV.
* **Cumulative Metrics:** Calculating and visualizing time-series metrics such as **Cumulative Conversion** and **Cumulative AOV** to monitor test progress.
* **Decision Making:** Translating statistical outputs (p-values and effect size) into clear, actionable business recommendations (Stop/Continue/Implement).

---

### **Next Steps / Recommendations**

* **Immediate Action:** Implement the changes tested in **Group B** immediately to all users to realize the statistically proven increase in Conversion Rate.
* **Future Roadmap:** Initiate the **RICE-prioritized hypothesis** (the one with the highest calculated score) as the next A/B test candidate.
* **Process Improvement:** Formalize a robust **outlier removal process** (using P95/P99 cutoffs) as a standard step in all future A/B test analyses to ensure the validity of statistical conclusions.
