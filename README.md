# 🇳🇬 Nigeria Food Inflation Tracker (Excel Project)

## Table of Contents
1. [Project Overview](#project-overview)  
2. [Key Questions Addressed](#key-questions-addressed)  
3. [Data Sources](#data-sources)  
4. [Key Skills, Formulas & Thought Process](#key-skills-formulas--thought-process)  
5. [Dashboard Features](#dashboard-features)  
6. [Excel Sheets Breakdown](#excel-sheets-breakdown)  
7. [Excel Functions & Formulas Used](#excel-functions--formulas-used)  
8. [Key Analytical Insights](#key-analytical-insights)  
9. [Strategic Relevance](#strategic-relevance)  
10. [About the Analyst](#about-the-analyst)  
11. [Let’s Collaborate](#lets-collaborate)  

---

## Project Overview
**Role Fit:** Data Analyst | Food Security & Policy | Socioeconomic Impact  
**Tool:** Microsoft Excel (Advanced)  
**Time Frame Analyzed:** Nov 2023–Nov 2024  
**Demo:** [Contact for dashboard walkthrough or screenshots]

This project investigates the surge in food prices across Nigeria, focusing on **regional disparities, affordability, and market risks**. Using recent market and wage data, it quantifies the real impact of inflation on households, highlights where and why prices are highest, and provides actionable insights for policymakers, NGOs, and business leaders.

> 💡 **Background**  
> As food prices soar, the gap between paycheques and the cost of a simple plate of food is widening for millions of Nigerians. This tracker analyzes the crisis, exposes regional and item-level inequities, and flags urgent areas for intervention.

---

## Key Questions Addressed
- **How much have staple food prices increased across Nigeria over the past year?**  
- **Which regions experience the highest price disparities for key staples?**  
- **What percentage of the minimum wage is required to afford a basic food basket?**  
- **Are there signs of price gouging in particular states or for specific foods?**  
- **Do conflict-affected zones like Borno and Adamawa have higher or lower prices than the national average?**  
- **Do port states (Lagos, Rivers) offer cheaper imported food prices compared to the national average?**
- **How is protein affordability changing and what does it mean for health?**

---

## Key Findings

- **A “one-unit shop” is now punishingly expensive:** Buying a single measure each of beans, onions, rice, yam, beef, and cooking oil costs roughly ₦11,200—about 16% of a ₦70,000 minimum wage—before you’ve even cooked a meal. A basic weekly food basket (beef, eggs, oil, yam, rice, beans) jumps to ₦17,462.17, or 25% of monthly income.
- **Regional price gaps are stark:** The South-East, South-West, and South-South post the highest prices for staples (₦2,500–₦3,100/kg for rice or beans), while the North-East, North-Central, and North-West are nearly 50% lower. A family in Onitsha or Ibadan may pay almost twice what a family in Bauchi or Sokoto pays for the same staple.
- **Price gouging is widespread:** States like Nasarawa (rice), Ebonyi/Kogi (fish), Enugu (potatoes), Niger (tomatoes), Gombe (onions), Abia (chicken), Imo (milk), Cross River (mudfish), and Kwara (catfish) show mark-ups exceeding twice the national average, often unrelated to transport or insecurity.
- **Conflict zones buck the trend:** In Borno and Adamawa, staples like yam, beans, and maize are actually cheaper than the national average—yam goes for about ₦885, roughly half the rate elsewhere, likely due to local harvests, subdued demand, and food aid. This is fragile and could change quickly if conflict disrupts supply.
- **Protein is becoming unaffordable:** Beef, fish, beans, and eggs are not only expensive but rising faster than other foods. Boneless beef is over ₦6,000/kg in most regions; dried catfish can exceed ₦12,000/kg in some states. Even beans now average over ₦2,700.

---

---

## Data Sources

- `selected_food_Nov_2024.xlsx` – Regional/state food price data (Nov 2023–Nov 2024)  
- National Bureau of Statistics (NBS) – Official inflation and wage data  
- Field market surveys and monitoring  

All datasets were **cleaned, standardized, and merged** in Excel for robust analysis.

---

## Key Skills, Formulas & Thought Process

| Skill Area                | Implementation Highlights                                                                 |
|---------------------------|-------------------------------------------------------------------------------------------|
| **Regional Disparity**    | Calculated Regional Equity Ratios for each staple food using:  
`=MAX($B2:$G2)/MIN($B2:$G2)` (Max regional price divided by Min regional price)            |
| **Affordability Analysis**| Modeled food basket cost as % of minimum wage (₦70,000/month) using:  
`= (Food Basket Cost / 70000) * 100`                                                        |
| **Inflation Tracking**    | Calculated Year-on-Year (YoY) inflation rates per item with:  
`= ((Price_CurrentYear - Price_PreviousYear) / Price_PreviousYear) * 100`                   |
| **Price Gouging Detection**| Flagged states/items with prices exceeding 1.5× the national average using:  
`=IF(StatePrice > 1.5 * NationalAvg, "Gouging", "Normal")`                                 |
| **Conflict Zone Analysis**| Compared conflict zone prices to national averages using direct subtraction and % difference:  
`= ((ConflictZonePrice - NationalAvg) / NationalAvg) * 100`                                |
| **Port Advantage Testing**| Benchmarked imported food prices in Lagos/Rivers vs. national average                    |
| **Pivot Tables & Charts** | Enabled dynamic regional/item analysis and visual storytelling                            |
| **Dashboard Design**      | Built clear visuals: bar, line, doughnut, and map charts                                  |
| **Summary Sheet**         | Created decision-maker-friendly insights and recommendations                              |

---

## Dashboard Features

- 📊 **Bar Charts** – YoY inflation by item, regional equity ratios, price gouging outliers  
- 📈 **Line Charts** – Price trends and regional comparisons  
- 🥧 **Doughnut Chart** – Food basket cost as % of minimum wage  
- 🗺️ **Map Visuals** – Regional disparities and conflict zone pricing  
- 📋 **Summary Panel** – Key takeaways, crisis alerts, and recommended actions  

---

## Excel Sheets Breakdown

| Sheet Name             | Purpose                                                                 |
|------------------------|-------------------------------------------------------------------------|
| `Regional Analysis`    | Matrix of staple prices by region, with equity ratios                   |
| `Port Access Advantage`| Imported food price comparison (Lagos/Rivers vs. national)              |
| `Price_gouging`        | Items/states with potential price gouging                               |
| `Food basket Afforda`  | Food basket affordability vs. minimum wage                              |
| `Conflict Zone`        | Borno/Adamawa staple prices vs. national average                        |
| `Summary/Insights`     | Key findings, charts, and policy recommendations                        |
| `Dashboard`            | Interactive visuals and slicers                                         |

---

## Excel Functions & Formulas Used

- `SUM`, `AVERAGE`, `MAX`, `MIN`: Core calculations for prices and ratios  
- `IF`: Conditional logic for flags and labels  
- `VLOOKUP`: Data merging and lookups  
- `SUMIF` / `SUMIFS`: Aggregated multi-criteria totals  
- Pivot Tables & Charts: Dynamic aggregation by region, item, and time  
- Conditional Formatting: Highlight crisis thresholds and outliers  
- Inflation Rate Formula (YoY):  


---

## Key Analytical Insights

- **Severely inflated staples** (beans, yam, onions, beef, oil) now cost up to 16% of monthly minimum wage for just one unit each while **food basket** i.e. food eaten on daily basis cahses 25% of the minimum wage leaving little for rent and others.
- **Regional price gaps** are stark: e.g., yam tuber costs 1.8× more in North Central than North East  
- **Price gouging** is evident in several states, with some items >2× national average  
- **Conflict zones** (Borno, Adamawa) buck the trend for grains/tubers, with prices up to 50% lower than national average  
- **Port states** (Lagos, Rivers) do not consistently offer cheaper imported food prices  

---

## Strategic Relevance

- Connects **market realities to food security and poverty risk**  
- Equips decision-makers with **targeted, data-driven recommendations**  
- Demonstrates **advanced Excel analytics, dashboarding, and storytelling**  
- Supports advocacy for **urgent policy action and market monitoring**  

---

## About the Analyst

**Lorreta Anyika**  
Founder @ **ALU Datatok** | Food Security & Policy Analyst | Excel | Data Storytelling  

📌 Specializes in translating complex market data into actionable insights  
📌 Experienced in regional and household-level economic analysis  
📌 Committed to using data for social impact and equity  

- 🔗 [LinkedIn](https://www.linkedin.com/in/uchechukwu-lorreta-anyika-7b5b4a253/)  
- 📹 [YouTube Channel – ALU Datatok](https://www.youtube.com/channel/UCQL3Wg_j3D5TWtn6ticnTsg)  
- 💬 [Join our WhatsApp Community](https://chat.whatsapp.com/LhAFCcplWbf0MYfyShJTgf)  

---

## Let’s Collaborate

This tracker turns complex food price data into clear, actionable insights for food security and policy.  
**If you’re hiring for roles in data analysis, policy, or advocacy—or want to partner on food systems work—let’s connect!**

> *Because behind every price tag is a family’s daily struggle—and a solution waiting to be found.*
