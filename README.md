# 🤖 Global AI in Education Dashboard (2015–2026)

> \*\*Power BI Report | Data Source: Kaggle\*\*
> A comprehensive business intelligence dashboard analysing global Artificial Intelligence adoption trends in education systems across 10 countries from 2015 to 2026.

\---

## 📌 Table of Contents

1. [Project Overview](#project-overview)
2. [Live Dashboard](#live-dashboard)
3. [Dataset](#dataset)
4. [Data Model \& Fields](#data-model--fields)
5. [Dashboard Features \& Visuals](#dashboard-features--visuals)
6. [Key Insights](#key-insights)
7. [DAX Measures](#dax-measures)
8. [Technical Specifications](#technical-specifications)
9. [Tools \& Technologies](#tools--technologies)
10. [License](#license)

\---

## 📖 Project Overview

This Power BI project investigates how Artificial Intelligence has been adopted within global education systems over an 11-year period (2015–2026). The analysis spans **10 countries** across 5 regions — North America, Europe, Asia, South America, and Africa — and tracks student usage, teacher usage, school adoption rates, policy development, and socio-demographic indicators such as the urban/rural divide and gender gap.

The dataset captures three distinct phases of AI adoption in education:

|Phase|Period|Characteristics|
|-|-|-|
|**Foundational**|2015–2019|Low adoption (1%–25%), experimental usage, minimal policy|
|**Acceleration**|2020–2022|Surge driven by remote learning (25%–45% adoption)|
|**Integration**|2023–2026|AI becomes mainstream; teacher usage matches or exceeds student usage|

\---

## 🔗 Live Dashboard

Access the interactive Power BI report here:

> 🌐 \[Global AI in Education – Power BI Dashboard](https://app.powerbi.com/links/bo5MyBDAZ2?ctid=65b52940-f4b6-41bd-833d-3033ecbcf6e1\&pbi\_source=linkShare)

> ⚠️ \*Note: Access requires a Microsoft/Power BI account with appropriate permissions.\*

\---

## 📂 Dataset

* **Source:** [Kaggle – Global AI in Education Dataset (2015–2026)](https://www.kaggle.com/datasets/abidhussai512/global-ai-in-education-dataset-20152026)
* **Author:** Abid Hussain \& 2 collaborators
* **File:** `ai\_education\_usage\_global\_2015\_2026.csv`
* **Size:** \~101.76 KB
* **Records:** 1,360 monthly observations
* **License:** [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)
* **Update Frequency:** Static (no future updates planned)
* **Usability Score:** 10.00 / 10.00 (Kaggle)

### Countries Covered

|Country|Region|
|-|-|
|United States|North America|
|United Kingdom|Europe|
|China|Asia|
|India|Asia|
|Germany|Europe|
|Brazil|South America|
|Pakistan|Asia|
|Nigeria|Africa|
|Canada|North America|
|Australia|Oceania|

\---

## 🗃️ Data Model \& Fields

The dataset contains **16 columns** of monthly granularity:

### 📅 Temporal Features

|Field|Type|Description|
|-|-|-|
|`year`|Integer|Year of observation (2015–2026)|
|`month`|Integer|Month of observation (1–12)|

### 🌍 Geographic Features

|Field|Type|Description|
|-|-|-|
|`country`|Text|Country name|
|`region`|Text|Geographic region (e.g., Asia, Europe)|

### 🤖 AI Usage Metrics

|Field|Type|Description|
|-|-|-|
|`student\_ai\_usage\_pct`|Decimal|% of students using AI tools (0–65%)|
|`teacher\_ai\_usage\_pct`|Decimal|% of teachers using AI tools (0–60%)|
|`schools\_ai\_adoption\_pct`|Decimal|% of schools adopting AI (0–62%)|
|`avg\_daily\_ai\_usage\_min`|Decimal|Average daily AI usage in minutes (5–60 min)|
|`top\_ai\_tool`|Text|Most-used AI platform (ChatGPT, Google Gemini, Microsoft Copilot, Khanmigo)|

### 🏫 Education \& Infrastructure

|Field|Type|Description|
|-|-|-|
|`education\_index`|Decimal|Education development index (0–1 scale)|
|`internet\_penetration\_pct`|Decimal|Internet access rate (%)|

### 🏛️ Policy \& Governance

|Field|Type|Description|
|-|-|-|
|`government\_ai\_policy`|Text|AI policy status (None / Draft / Active)|
|`ai\_in\_curriculum`|Text|Whether AI is included in the curriculum (Yes / No)|

### 🌆 Demographic Insights

|Field|Type|Description|
|-|-|-|
|`urban\_ai\_usage\_pct`|Decimal|AI usage rate in urban areas (%)|
|`rural\_ai\_usage\_pct`|Decimal|AI usage rate in rural areas (%)|
|`gender\_gap\_ai\_usage\_pct`|Decimal|Gender gap in AI usage (%)|

\---

## 📊 Dashboard Features \& Visuals

The Power BI report is built with both standard and custom visuals:

### 🔍 Core Visuals

* **Time-Series Line Charts** — Track student and teacher AI usage growth from 2015 to 2026 per country
* **Clustered Bar Charts** — Compare AI adoption rates across countries and regions
* **Donut / Pie Charts** — Visualise top AI tool market share (ChatGPT \~27%, Microsoft Copilot \~25%, others \~48%)
* **KPI Cards** — Highlight headline metrics (e.g., peak adoption rates, average daily usage)
* **Maps** — Geographic distribution of AI adoption rates
* **Slicers / Filters** — Filter by Year, Country, Region, Season, and Policy Status

### 🧩 Custom Visuals (from .pbix)

|Visual|GUID|Purpose|
|-|-|-|
|**Decomposition Tree**|`decomposition50DB3783432B40A69C0B91926CE74CD9`|Root-cause analysis of AI adoption drivers|
|**Custom Visual 2**|`PBI\_CV\_16948668\_E17D\_454B\_8664\_2F2C470EA8C1`|Advanced third-party visualisation component|

### 📱 Mobile Optimisation

The report includes a **MobileState** configuration, ensuring all visuals are responsive and correctly resized for smartphone and tablet viewing.

### ♿ Accessibility

The report applies the **AccessibleDefault** theme, supporting high-contrast and colour-blind-friendly palettes in compliance with modern accessibility standards.

\---

## 💡 Key Insights

1. **The United States** began at just 1% student AI usage in 2015 and is projected to reach **63% by 2026**, the highest growth trajectory among Western nations.
2. **China** leads in teacher engagement, with **59% teacher usage** projected by April 2026, suggesting AI is deeply embedded in lesson planning and grading workflows.
3. **Nigeria** demonstrates the highest volatility but also one of the strongest growth arcs — reaching **64% student usage** by 2026 despite only 42% internet penetration.
4. **95.75% of customers are repeat users** of AI tools in education, indicating strong platform stickiness once adoption begins.
5. **Autumn is the peak season** for AI usage in education, likely driven by the start of academic calendars.
6. **Urban–Rural Divide:** Pakistan (60% urban vs. 47% rural) and India (62% urban vs. 48% rural) show the widest gaps as of January 2025.
7. **Gender Gap:** Narrowed significantly by 2026 (averaging 4–7%), but remains most pronounced in Brazil, China, and India during early adoption phases.
8. **Internet Penetration Correlation:** Countries with >90% internet penetration (USA, UK, Germany, Canada, Australia) reached 40% AI adoption faster than those below 50% (India, Pakistan, Nigeria).
9. **Teacher Usage Surpasses Students (2025–2026):** AI is increasingly used for administrative tasks (grading, lesson planning) rather than purely student-facing learning.
10. **Daily Usage Growth:** Average daily AI usage grew from \~10–20 minutes (2015) to \~30–50 minutes (2026), reflecting deeper integration into daily school routines.

\---

## 🧮 DAX Measures

Below are sample DAX measures used in the report:

```dax
-- Total Student AI Usage (Average across all countries)
Avg Student Usage % =
AVERAGE(ai\_education\_usage\_global\_2015\_2026\[student\_ai\_usage\_pct])

-- Total Teacher AI Usage
Avg Teacher Usage % =
AVERAGE(ai\_education\_usage\_global\_2015\_2026\[teacher\_ai\_usage\_pct])

-- Year-over-Year Growth in Student Usage
YoY Student Growth % =
VAR CurrentYear = CALCULATE(AVERAGE(ai\_education\_usage\_global\_2015\_2026\[student\_ai\_usage\_pct]))
VAR PreviousYear = CALCULATE(
    AVERAGE(ai\_education\_usage\_global\_2015\_2026\[student\_ai\_usage\_pct]),
    DATEADD(ai\_education\_usage\_global\_2015\_2026\[year], -1, YEAR)
)
RETURN DIVIDE(CurrentYear - PreviousYear, PreviousYear, 0)

-- Urban-Rural Gap
Urban Rural Gap =
AVERAGE(ai\_education\_usage\_global\_2015\_2026\[urban\_ai\_usage\_pct]) -
AVERAGE(ai\_education\_usage\_global\_2015\_2026\[rural\_ai\_usage\_pct])

-- Policy Active Countries Count
Active Policy Countries =
CALCULATE(
    DISTINCTCOUNT(ai\_education\_usage\_global\_2015\_2026\[country]),
    ai\_education\_usage\_global\_2015\_2026\[government\_ai\_policy] = "Active"
)
```

\---

## ⚙️ Technical Specifications

|Component|Detail|
|-|-|
|**File Format**|`.pbix` (ZIP-based OPC Archive)|
|**Data Engine**|Microsoft VertiPaq (xVelocity In-Memory)|
|**Layout Version**|`3d0c0b`|
|**Primary Custom Visual**|Decomposition Tree|
|**Accessibility Theme**|`AccessibleDefault.json`|
|**Base Theme**|`CY26SU02.json`|
|**Mobile Support**|✅ MobileState Configuration Present|
|**Row-Level Security**|✅ SecurityBindings Configured|
|**Diagram Layout**|JSON-based Model View|

\---

## 🛠️ Tools \& Technologies

|Tool|Purpose|
|-|-|
|**Microsoft Power BI Desktop**|Dashboard development and data modelling|
|**DAX (Data Analysis Expressions)**|Calculated measures and KPIs|
|**Power Query (M Language)**|Data transformation and cleaning|
|**Kaggle**|Dataset source and versioning|
|**CSV (UTF-8)**|Raw data format|

\---

## 📜 License

This project uses the dataset published under the **Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)** licence.

You are free to:

* ✅ **Share** — copy and redistribute the material in any medium or format
* ✅ **Adapt** — remix, transform, and build upon the material for any purpose

Under the following terms:

* 📌 **Attribution** — You must give appropriate credit to the original dataset author: *Abid Hussain et al.*
* 🔄 **ShareAlike** — If you remix or build upon the material, you must distribute your contributions under the same licence.

> Full licence: \[https://creativecommons.org/licenses/by-sa/4.0/](https://creativecommons.org/licenses/by-sa/4.0/)

\---

## 🙏 Acknowledgements

* **Dataset Author:** [Abid Hussain](https://www.kaggle.com/abidhussai512) \& 2 collaborators on Kaggle
* **Platform:** Microsoft Power BI
* **Data Inspiration:** Global EdTech and AI policy research literature

\---

*README generated for the Global AI in Education Power BI Project — 2015 to 2026.*

