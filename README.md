# HYBE Financial Performance Dashboard 2024

This is an **investor-style financial analysis dashboard** of Hybe Co., Ltd (the biggest South Korean Entertainment Company), built using publicly available financial disclosures from HYBE. My objective behind this project was to integrate my interests with data analysis and thus, I created this dashboard to transform raw financial statements into **structured, interactive dashboards** that can be understood by stakeholders and investors. 

The project covers HYBE’s financial performance in the FY 2024, and comparison with FY 2023. 

## Data Source

* Financial statement was extracted directly from **HYBE’s official website** -> https://hybecorp.com/eng/ir/archive/result?lang=eng
* Quarterly data chosen up to **FY 2024**
* Original dataset was provided in **Korean**

---

## Methodology

### 1. Data Collection & Translation

* Financial data was downloaded directly from HYBE’s official disclosures.
* The dataset was originally in Korean and required translation prior to analysis.
* Initial translation was performed using **Papago** but few metrics were translated generically or ambiguously.
* To ensure accuracy and business relevance, translations were refined using **ChatGPT**. This ensured alignment with standard financial analysis conventions rather than literal translations.
<img width="1268" height="520" alt="image" src="https://github.com/user-attachments/assets/fe138e3c-7ef5-4b45-b241-ee82c5b1b245" />

---

### 2. Data Reshaping & Transformation

* The original dataset had a **wide format**, with separate columns for each quarter.
* Using **Excel Power Query / Power Pivot**, the data was transformed into a **long (tidy) format** through unpivoting.
* This resulted in one row per metric per quarter. 
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
* Developed KPIs mostly used in investor and stakeholder analysis

I focused on understanding which metrics matter most in evaluating a company's performance rather than just reporting numerical values.

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
----
REVENUE DASHBOARD

<img width="728" height="336" alt="image" src="https://github.com/user-attachments/assets/7ea5d993-90a3-414d-8a8d-31f99cf510f9" />

----
EXPENSES DASHBOARD

<img width="765" height="350" alt="image" src="https://github.com/user-attachments/assets/06689203-0645-41dd-9bf7-ed3262b7e210" />

----
PROFITS DASHBOARD

<img width="714" height="336" alt="image" src="https://github.com/user-attachments/assets/7e571e60-8c54-4f56-a619-a8e52ebaf68e" />

---

### 8. Interactivity

* Implemented **Excel Macros and basic VBA** to create navigation buttons that allow seamless transitions between Revenue, Expense, and Profit dashboards
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
- Total Revenue increased by **3.56%** from 2023, despite BTS' hiatus. This indicates multi-label strategy is successful.
- Highest Quarterly Revenue in FY 2024 Q4 - ₩ 7,26,419 billion
- **Albums** were the primary revenue drivers, followed by **Concert Revenue** (#2) and **Merchandise & Licensing** (#3)
- Operating Expenses increased in 2024, indicating a deliberate aggressive expansion phase.
- Operating Expense Ratio of 0.91 indicates that from every ₩ 1 of revenue, ₩ 0.91 is spent on operating costs.
- High operating cost also indicates short term margin pressure is present as company absorbs costs before revenue realization.
- COGS is the highest expense category indicating expenses are majorly for revenue generating activities rather than administration overhead
- SG&A increased due to debut of 3 groups debut marketing activities.
- Non-operating expenses and Corporate Tax decreased, partially offsetting the impact of operating expenses growth.
- Expenses volatility is proportional to business cycles like artist's music, concert schedule not due to structural ineffeciency.
- Hybe recorded net loss in profits, decreasing up to 102%. This is reportedly due to non-operating valuation losses on equity investments like SM Entertainment.
- Operating Profit is volatile and aligns with front-load investment patterns like music release and concert schedules.
- Gross Profit Margin is 42.5% i.e it is stable but operating income decreased and net income further declined. 

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
