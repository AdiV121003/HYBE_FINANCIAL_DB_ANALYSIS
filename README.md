# HYBE Financial Performance Dashboard (FY 2023–FY 2025 Q2)

This is an **investor-style financial analysis dashboard** of Hybe Co., Ltd (the biggest South Korean Entertainment Company), built using publicly available financial disclosures from HYBE. My objective behind this project was to integrate my interests with data analysis and thus, I created this dashboard to transform raw financial statements into **structured, interactive dashboards** that can be understood by stakeholders and investors. 

The project covers HYBE’s financial performance from **FY 2023 to FY 2024**, with **FY 2025 data available up to Q2 (YTD)**.

**(Note: On the date of project release, Hybe 2025 Q3 data was also available but at the time of project creation and analysis, only the FY 2025 Q2 data was available)
**---

## Data Source

* Financial statements sourced from **HYBE’s official website** -> https://hybecorp.com/eng/ir/archive/result?lang=eng
* Quarterly data chosen up to **FY 2025 Q2**
* Original dataset was provided in **Korean**

---

## Methodology

### 1. Data Collection & Translation

* Financial data was downloaded directly from HYBE’s official disclosures.
* The dataset was originally in Korean and required translation prior to analysis.
* Initial translation was performed using **Papago** but few metrics were translated generically or ambiguously.
* To ensure accuracy and business relevance, translations were refined using **ChatGPT**. This ensured alignment with standard financial analysis conventions rather than literal translations.
  ///canva image

---

### 2. Data Reshaping & Transformation

* The original dataset had a **wide format**, with separate columns for each quarter.
* Using **Excel Power Query / Power Pivot**, the data was transformed into a **long (tidy) format** through unpivoting.
* This resulted in:

  * One row per metric per quarter
I performed this step to improve ease of calculations and analysis.

---

### 3. Time Dimension Engineering

* The original time identifier followed the format:
  `Year.Quarter` (e.g., 2024.Q2)
* A separate **Quarter** column was derived by extracting the quarter component (e.g., Q2).
---

### 4. Financial Categorization

To perform structured analysis, I created a **Category** column to classify financial metrics into four groups:

* **Revenue**
* **Expenses**
* **Profit**
* **Equity**

This enabled me to perform category-based filtering and analysis. It also helped me create seperate analytical views - from revenue, profits and expenses POV. 

---

### 5. Financial Analysis & KPI Development

* Conducted exploratory analysis using **PivotTables and PivotCharts**.
* Developed KPIs mostly used in investor and stakeholder analysis, including:

  * Revenue and profitability indicators 
  * Expense efficiency measures
  * Quarterly and yearly performance comparisons
* I focused on understanding which metrics matter most in evaluating a company's performance rather than just reporting numerical values.

---

### 6. Cross-Verification & Financial Validation

I validated my calculations and insights by referencing:

  * **Yahoo Finance**
  * **MarketWatch**
  * Public financial summaries and analyst discussions

* Used **Google Gemini** to:
  * Clarify financial terminology
  * Verify formula logic
  * Cross-check metric definitions against standard financial practices
---
### 7. Dashboard Design & Storytelling

* Built interactive dashboards designed from an **investor-oriented perspective** and applied intuitive aesthetic design principles to maintain visual hierarchy.
* I made use of cohesive color theme inspired by HYBE/BTS branding
* Integrated brand-relevant visuals (logos and artist imagery)
<img width="1094" height="502" alt="image" src="https://github.com/user-attachments/assets/fcf4c478-4e51-49e7-b802-d63ff36661a2" />


<img width="1046" height="464" alt="image" src="https://github.com/user-attachments/assets/0e2dbeed-a443-49bd-9708-39fd444de3ad" /> 


Profits Dashboard: 

<img width="1037" height="477" alt="image" src="https://github.com/user-attachments/assets/3a6aea39-7ce8-45f5-a96c-b1104d9e62a7" />



---

### 8. Interactivity

* Implemented **Excel Macros and basic VBA** to:

  * Create navigation buttons that allow seamless transitions between Revenue, Expense, and Profit dashboards
---

## Tools & Technologies

* **Microsoft Excel**

  * Power Query / Power Pivot
  * PivotTables & PivotCharts
  * Slicers
  * Macros & VBA
* **Naver Papago** – initial Korean-to-English translation
* **ChatGPT & Google Gemini** – contextual translation refinement, financial validation
* **Public financial platforms** – Yahoo Finance, MarketWatch

---

## Data Coverage & Limitations

* FY 2025 financial data is available only up to **Q2 (YTD)**.
* Partial-year data is clearly labeled throughout the analysis to avoid misinterpretation.
* All analysis is based on publicly available disclosures and secondary validation sources.

---

## INSIGHTS AND INTERPRETATION:

> *This section will be expanded to include key insights and investor-oriented interpretations derived from the dashboards.*

---

## Project Outcome

This project demonstrates my ability to:

* Transform raw, multilingual financial disclosures into structured analytical datasets
* Apply financial reasoning and validation to ensure analytical reliability
* Build interactive, investor-style dashboards that support decision-oriented analysis

  Basically, my purpose of integrating my interests with data analysis process was successful. I thorougly enjoyed the entire process and realised my own talents for data analysis and especially dashboard making 🥳
---

### 📌 Note

This project is intended for educational and analytical purposes, not for any investment advice.
