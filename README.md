# **Sudan Humanitarian Analytics Dashboard**

![Home page](/sudan-dashboard-portfolio/screenshots/001_home.PNG)

**One-line summary**  
*Interactive Power BI dashboard linking conflict events, displacement, market prices, demographics, and GDP to show where violence, displacement, and market stress intersect across Sudan.*

---

## **Demo video**
https://github.com/user-attachments/assets/31c92aaa-234b-44ef-9736-210ff9a36d28

*Short walkthrough showing navigation, slicers, bookmarks, and interactive exploration of the report.*

---

## **Quick project note (read first)**  
This repository is a **portfolio demonstration**. The visuals show methods, data engineering, and storytelling — not an official source. Data coverage varies by dataset and year; see the *Data notes* section below for details.

---

## **How this README is organized**  
1. Visuals (one screenshot per page) with short, clear explanations.  
2. A short technical summary and skills list.  
3. Data notes and limitations.  
4. How to view the demo and files included.  

---

## **Page 1 — Home (overview)**

![Home page](/sudan-dashboard-portfolio/screenshots/01_home.PNG)

**Caption:** *Overview: headline KPIs and a switchable trend for national framing.*  

**What this page shows (2–3 sentences)**  
The Home page presents the headline metrics: **People in Need**, **Internally Displaced**, **People Facing Acute Food Insecurity**, and **2025 GDP**. 

A central interactive map highlights the geographic location of humanitarian hotspots across the region to illustrate current needs and reach. Use this page to get a quick, high-level sense of the crisis scale and to visualize the areas requiring the most critical assistance.

**What to look for**  
- Headline KPI cards for high-level crisis metrics.  
- Color-coded map markers indicating distinct levels of regional need.  
- Top navigation to move to each detailed page.

---

## **Page 2 — Conflict**

![Conflict page](/sudan-dashboard-portfolio/screenshots/02_conflict.PNG)

**Caption:** *Conflict: state-level intensity and top states by event counts.*  

**What this page shows (2–3 sentences)**  
A map highlights conflict intensity by state and a ranked bar chart lists the top states by event counts. KPI cards summarize event totals and fatalities for the selected period. This page helps identify geographic hotspots and the scale of violence driving humanitarian needs.

**Key visuals explained**  
- **Conflict intensity map:** circle size and color show relative event intensity by state.  
- **Top states bar chart:** ranked counts to quickly see where events concentrate.  
- **KPI cards:** quick totals for events, violence against civilians, and fatalities.

---

## **Page 3 — Displacement**

![Displacement page](/sudan-dashboard-portfolio/screenshots/03_displacement.PNG)

**Caption:** *Displacement: IDP stocks by state and origin→destination flows.*  

**What this page shows (2–3 sentences)**  
State-level IDP stocks are shown on a map and a Sankey flow diagram shows origin→destination movement between states. Cards summarize total IDPs, returnees, and vulnerable subgroups (children, women). Use this page to understand who is displaced, where they are, and the main movement corridors.

**Key visuals explained**  
- **IDP stock map:** size-coded circles show where IDPs are concentrated.  
- **Sankey flow:** visualizes major flows from origin states to hosting states.  
- **Demographic cards:** quick counts for children and women among IDPs.

---

## **Page 4 — Food Security**

![Food Security page](/sudan-dashboard-portfolio/screenshots/04_food_security.PNG)

**Caption:** *Food Security: market price trends and annual sorghum price volatility.*  

**What this page shows (2–3 sentences)**  
Small multiples show market price trends across key markets and a larger chart shows year‑on‑year volatility for sorghum (a staple). Cards highlight the number of people in emergency and catastrophe and the percent above 5‑year average for key staples. This page links market stress to conflict and displacement patterns.

**Key visuals explained**  
- **Market small multiples:** each market’s price trend for quick comparison.  
- **Volatility chart:** YoY percent changes to show instability and spikes.  
- **Food security KPIs:** people in emergency/catastrophe and price deviation from historical averages.

---

## **Page 5 — Demographics**

![Demographics page](/sudan-dashboard-portfolio/screenshots/05_demographics.PNG)

**Caption:** *Demographics: population pyramid and age-group distribution by state.*  

**What this page shows (2–3 sentences)**  
A population pyramid shows age and sex structure; stacked bars compare age groups across states. Cards show total population, growth rate, median age, and dependency ratio. This page highlights vulnerability shaped by a young population and regional differences in child share.

**Key visuals explained**  
- **Population pyramid:** visual age/sex structure for national context.  
- **Age groups by state:** where child shares and working-age populations concentrate.  
- **Demographic KPIs:** quick reference for population size and growth.

---

## **Page 6 — Economy**

![Economy page](/sudan-dashboard-portfolio/screenshots/06_economy.PNG)

**Caption:** *Economy: GDP level, YoY growth, per-capita, and indexed comparisons.*  

**What this page shows (2–3 sentences)**  
GDP level and growth trends are shown alongside per-capita figures and a relative GDP index (base 2015 = 100) that compares Sudan’s growth trajectory to the two highest and two lowest performers each year. Use this page to see macro trends and how Sudan’s recovery or decline compares to peers.

**CAGR explanation**  
**Compounded Annual Growth Rate (CAGR)** measures the average yearly growth rate of Sudan’s GDP over a period, smoothing out ups and downs. Here it shows the typical annual change since South Sudan separated (2011/2012). A negative CAGR means the economy has, on average, shrunk each year since that date; a positive CAGR means it has, on average, grown.

**Relative GDP Index**  
**Purpose:** Compare Sudan’s GDP path against the world's two largest and two smallest economies (by absolute GDP value) each year, indexed to a 2015 = 100 base to track and normalize their relative growth rates.

**How to read it:** an index value above 100 means GDP has grown since 2015; below 100 means it has fallen. This is a **relative** measure of change, not absolute size. A country with a small economy can show a large index increase (big percent growth) while still having a much smaller total GDP in dollars. Use the index to compare growth **trajectories**; use raw GDP values to compare absolute economic size.

---

## **Page 7 — Detail (bookmark-driven parameters)**

![Detail page](/sudan-dashboard-portfolio/screenshots/07_detail.PNG)

**Caption:** *Detail: bookmark-driven parameter page and raw tables for audit.*  

**What this page shows (2–3 sentences)**  
The Detail page is a parameterized view built with bookmarks. The default screenshot shows the **Total Population** parameter. Other parameters (Total Events, Total Fatalities, Total IDPs, Total Returnees) switch the page to show related slicers and filters. Only the default screenshot is included in this repo to keep the README concise.

**How the bookmarks work (simple list)**  
- **Default (Total Population):** shows population-related filters (region, gender, age band) and the map view.  
- **Total Events:** switches to event-related slicers and the map view.  
- **Total Fatalities:** shows fatality metrics and the map view.  
- **Total IDPs:** shows IDP-specific slicers and the map view.  
- **Total Returnees:** shows returnee filters and the map view.  

*Note:* The bookmarks let a user change the page layout and filters without leaving the Detail page. This keeps the map view and parameter views in one place for easy auditing.

---

## **Skills demonstrated**
**Data engineering & databases:** PostgreSQL, schema design, ETL, CSV handling, GeoJSON prep.  
**SQL & transformations:** data cleaning, unpivoting, joins, LOOKUPVALUE patterns.  
**Modeling:** star schema, dimension and fact tables, surrogate keys.  
**Power BI:** Power Query, data modeling, DAX (row-aware measures, conditional aggregation), tooltips, small multiples, maps, Sankey.  
**Design & storytelling:** KPI hierarchy, trend switching, focused tooltips, accessible color choices, readable layouts.  
**Quality & auditability:** diagnostic tables, hidden checks, explicit handling of nulls and missing data.

---

## **Design choices and accessibility**  
- **Readable over flashy:** fonts, spacing, and clear KPI cards were prioritized so readers can scan quickly.  
- **Color and contrast:** chosen for clarity and to work for common forms of color vision deficiency.  
- **Tooltips and small multiples:** provide detail on demand without cluttering the page.  
- **Bookmarks for audit:** the Detail page groups raw tables and parameter views so analysts can validate measures easily.

---

## **Data notes and limitations (must read)**  
- This project is a **demonstration** and should **not** be used as an authoritative source.  
- Datasets cover different years and are not fully aligned: population (2024), IDPs/returnees (2025), conflict events (1997–2026), GDP (1975–2025).  
- Year-aware measures were implemented to reduce mixing of historical events with current market data.  
- Where external benchmarks exist (for example, World Bank GDP series), the dashboard’s GDP trends are consistent with those sources.

---

## **Files included**
- `README.md` — this file.    
- `demo-video.mp4` — short walkthrough recorded with OBS.  
- `screenshots/` — 7 images named in this README.  
---

## **Author**
**Author:** [Ahmed Elhassan]      
**Last updated:** [12-June-2026]
